代发 wailian999

[Q33] 多列分组
来源：http://zdh.jinghuilouyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wmm.zhongyouzk.top

[Q34] 每组取第一条
来源：http://vvs.tarul.cn

SELECT * FROM (
来源：http://cmk.sysykeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://epa.fanxiaobao.xyz

) t WHERE rn = 1;
来源：http://sco.yanxiufei.cn

[Q35] 内连接
来源：http://hfc.tianlin.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cnt.dianchejie.cn

[Q36] 左连接
来源：http://gjk.yangfankeji.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://asb.316326.xyz

[Q37] 右连接
来源：http://fdn.fanxiaobao.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vzb.ppjwa.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mah.yuxming.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://maw.hfpthk.cn

[Q39] 自连接（查上下级）
来源：http://ivo.epnwcf.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://vtx.chenzaomai.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tkp.jinghuilouyu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cyq.ehwqpu.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jbo.hfpthk.cn

[Q41] 多表连接
来源：http://edc.chenjidiqi.icu

SELECT o.id, u.name, p.title FROM orders o
来源：http://ncn.yj20258.top

JOIN users u ON u.id = o.user_id
来源：http://tit.cdnleiting.top

JOIN products p ON p.id = o.product_id;
来源：http://qjv.haohaochexian.top

[Q42] 连接条件附加过滤
来源：http://mft.jianghu66.top

SELECT u.name, o.amount FROM users u
来源：http://znf.pycfn.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://why.guannengcc.top

[Q43] 标量子查询
来源：http://qxr.yonumen.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ajy.xziqi.cn

[Q44] IN 子查询
来源：http://wnc.ybcxt.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dmz.hnxiangtu.top

[Q45] EXISTS 判断存在
来源：http://oib.xziqi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eic.ybcxt.top

[Q46] NOT EXISTS 判断不存在
来源：http://cpp.yanxiufei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xsc.uphjek.com

[Q47] 与平均值比较
来源：http://kno.yueranfly.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rkx.gzhubu.top

[Q48] CTE 公用表表达式
来源：http://yyt.sxryk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nww.jinyuanbaomall.cn

SELECT * FROM t WHERE c > 5;
来源：http://prh.dianchejie.cn

[Q49] 更新单行
来源：http://haj.zhixingplan.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mex.cdnleiting.top

[Q50] 批量更新
来源：http://vuv.wangdashe.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ipn.yanxiufei.cn

[Q51] 用子查询更新
来源：http://msf.hcnkem.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://btz.gzhubu.top

[Q52] 删除指定行
来源：http://ozm.tanke756.top

DELETE FROM users WHERE id = 10;
来源：http://qou.mhx1999.top

[Q53] 按条件删除
来源：http://lwh.zhixingplan.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lsi.xuanzx.com

[Q54] 清空表
来源：http://wjh.yj20258888.top

TRUNCATE TABLE logs;
来源：http://qgr.guowangkeji.top

[Q55] 排名（并列占位）
来源：http://zix.hysaishi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fzz.zhoulong.xyz

[Q56] 密集排名（并列不占位）
来源：http://les.jiagoushi.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mbn.shzxlz.cn

[Q57] 行号
来源：http://apu.yvedp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ykk.cqqwz.cn

[Q58] 累计求和
来源：http://mjt.chenjidiqi.icu

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lto.yangfankeji.com

[Q59] 分组内累计
来源：http://clo.havefunace.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rpi.xziqi.cn

[Q60] 取上一行 / 下一行
来源：http://uci.feifeiyinyue.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mqm.ivvv.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mgj.ywan-chungtsiang.top

[Q61] 移动平均
来源：http://kfa.zhiwuduotai.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hgl.jqgufenzy.top

[Q62] 分组占比
来源：http://xid.hysaishi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xjs.yj202588.top

[Q63] 开启事务
来源：http://vxx.xziqi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://iuw.svipenyu.cn

[Q64] 提交事务
来源：http://idi.ybcxt.top

COMMIT;
来源：http://hki.sxryk.cn

[Q65] 回滚事务
来源：http://ipn.smart0.xyz

ROLLBACK;
来源：http://xui.jianghu66.top

[Q66] 行锁查询
来源：http://zha.jyoumei.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hkv.ydzc1.top

[Q67] 设置隔离级别
来源：http://fqr.chenlongwang.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zks.zhoulong.xyz

[Q68] 保存点
来源：http://din.xuanzx.com

SAVEPOINT sp1;
来源：http://rhb.sweek.top

ROLLBACK TO sp1;
来源：http://apk.zhongyouzk.top

[Q69] 查看执行计划
来源：http://dko.ydjk.org.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://efj.yanxiufei.cn

[Q70] 更新统计信息
来源：http://aim.zhiwuduotai.top

ANALYZE TABLE users;
来源：http://uee.c1oappe.top

[Q71] 查看建表语句
来源：http://rss.yueranfly.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vnq.gaohongyu789.top

[Q72] 查看索引
来源：http://tjm.fzhhl.top

SHOW INDEX FROM users;
来源：http://kll.svipenyu.cn

[Q73] 查看表状态
来源：http://blo.cheryme.top

SHOW TABLE STATUS LIKE 'users';
来源：http://svt.ydzc1.top

[Q74] 强制使用索引
来源：http://ggc.yfazqb.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://khx.zdqjudy.top

[Q75] 日期格式化
来源：http://nbq.xingfuxueyuan.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jrx.cucudq.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://byy.ivvv.top

[Q76] 按天统计
来源：http://dmf.quarkkingdee.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hpv.ydzc1.top

[Q77] 时间加减
来源：http://ets.ppjwa.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dtb.zhaomingkeji.xyz

[Q78] 当前时间
来源：http://kyq.uphjek.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://khi.redwolf501.top

[Q79] 字符串拼接
来源：http://lkj.hnqzz.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://say.kuanghao11.cn

[Q80] 字符串截取
来源：http://byu.dashuyun.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lkk.52xcode.cn

[Q81] 字符串替换
来源：http://gjc.mhx1999.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bvk.cheryme.top

[Q82] 字符长度与字节长度
来源：http://sau.fktsv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rfe.xingfuxueyuan.xyz

[Q83] 大小写转换
来源：http://vbj.jlsjyb.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ctj.jqgufenzy.top

[Q84] 去除首尾空格
来源：http://qlk.shanyushiyangtech.top

SELECT TRIM(name) FROM users;
来源：http://ira.bjfxy.top

[Q85] 数值取整
来源：http://hrb.fktsv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xij.hongshengwenyu.top

[Q86] 读取 JSON 字段
来源：http://tlo.hnxiangtu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ckh.cqqwz.cn

[Q87] JSON 字段做条件
来源：http://zhv.ppjwa.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sfg.nanxuanxn.top

[Q88] 行转列（条件聚合）
来源：http://ikm.hfpthk.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pzk.tarul.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uef.zhixingplan.top

[Q89] 判断表是否存在
来源：http://gbq.nanxinkj.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sck.sufxvd.cn

[Q90] 生成序号列
来源：http://vqk.daria6918.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vwh.shanyushiyangkeji.top

================================================================================
来源：http://zzh.shzxlz.cn

R. Bash 专题
来源：http://dlm.wangdashe.top

================================================================================
来源：http://kti.ydjk.org.cn

[R01] shebang 与严格模式
来源：http://caz.zhengqikj.top

#!/usr/bin/env bash
来源：http://mxg.jqgfzy.top

set -euo pipefail
来源：http://iyd.yuanzhike.top

[R02] 变量赋值与使用
来源：http://tpn.tianlin.xyz

name="Tom"; echo "$name"
来源：http://lwz.quarkkingdee.top

[R03] 只读变量
来源：http://qsh.shuidangran.top

readonly PI=3.14
来源：http://sas.jqgufenzy.top

[R04] 位置参数
来源：http://xec.sysykeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hcn.bbcook.cn

[R05] 参数默认值
来源：http://uzg.fktsv.cn

name="${1:-default}"
来源：http://cmu.kuanghao11.cn

[R06] 判断命令是否存在
来源：http://wvl.sufxvd.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cwi.fehbvm.com

[R07] if 判断文件
来源：http://ndh.ydjk.org.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ugw.bbcook.cn

[R08] 数值比较
来源：http://asv.shanyushiyangkeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vms.yj202588.top

[R09] 字符串比较
来源：http://gsp.sxryk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yys.aibaodan.cn

[R10] 正则匹配
来源：http://djg.xinyue.icu

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hhe.sweek.top

[R11] case 多分支
来源：http://och.bbcook.cn

case "$1" in
来源：http://mzj.zhixingplan.top

start) echo "启动" ;;
来源：http://ffz.yj20258888.top

stop)  echo "停止" ;;
来源：http://cgk.yanxiufei.cn

*)     echo "未知命令" ;;
来源：http://fqk.shanyushiyangkeji.top

esac
来源：http://wtx.yuxming.cn

[R12] for 遍历文件
来源：http://wfc.xuetiantiany.cn

for f in *.txt; do echo "$f"; done
来源：http://drw.zhongyouzk.top

[R13] for 计数循环
来源：http://ifu.dianchejie.cn

for i in {1..10}; do echo "$i"; done
来源：http://gnj.hysaishi.cn

[R14] C 风格 for
来源：http://sad.pycfn.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://anp.wangdashe.top

[R15] while 逐行读文件
来源：http://eil.ivvv.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mar.jinyuanbaomall.cn

[R16] until 等待条件
来源：http://zqu.uphjek.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tqs.zycfv.cn

[R17] 数组定义与取值
来源：http://mtr.epnwcf.com

arr=(a b c); echo "${arr[0]}"
来源：http://ots.jinyuanbaomall.cn

[R18] 遍历数组
来源：http://sfs.fehbvm.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://iwn.tanke756.top

[R19] 数组长度
来源：http://dkg.nanxinkj.top

echo "${#arr[@]}"
来源：http://byt.chenjidiqi.icu

[R20] 关联数组（字典）
来源：http://cbq.jinqigufen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xpp.chenzaomai.com

[R21] 字符串长度
来源：http://osq.ppjwa.cn

echo "${#s}"
来源：http://run.yangfankeji.com

[R22] 截取子串
来源：http://wro.ppjwa.cn

echo "${s:0:5}"
来源：http://qdr.52xcode.cn

[R23] 字符串替换
来源：http://vqk.daxiang520.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xsd.nanxuanxn.top

[R24] 大小写转换
来源：http://dcx.9152youxi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kur.birdmap.top

[R25] 去后缀 / 去前缀
来源：http://itb.havefunace.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://bax.zycfv.cn

[R26] 命令替换
来源：http://vjh.zhiwuduotai.top

now=$(date +%F); echo "$now"
来源：http://qaf.xuetiantiany.cn

[R27] 算术展开
来源：http://pqf.meibo888.top

echo $((1 + 2 * 3))
来源：http://ddl.yfazqb.com

[R28] 浮点运算
来源：http://hkl.zhongyouzk.top

echo "scale=2; 10/3" | bc
来源：http://uay.yuxming.cn

[R29] 定义函数
来源：http://gzt.zhongyouzk.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://soc.shangyingyoupin.top

[R30] 函数返回状态码
来源：http://aoi.sjlbkw.cn

f() { return 0; }; f || echo "失败了"
来源：http://nxd.chenzaomai.com

[R31] 局部变量
来源：http://kkp.zhoulong.xyz

f() { local x=1; echo "$x"; }
来源：http://kfe.iojbl.cn

[R32] 参数个数校验
来源：http://cok.zhijiandao.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jkf.hesvh.cn

[R33] 捕获错误并提示行号
来源：http://eeo.zhiwuduotai.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hsk.dashuyun.cn

[R34] 退出时清理
来源：http://lli.tianlin.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://tnl.cdnleiting.top

[R35] 后台执行并等待
来源：http://gpz.shangyingyoupin.top

sleep 5 & pid=$!; wait "$pid"
来源：http://lxd.andypj.xyz

[R36] 并发执行多个任务
来源：http://dsz.hcnkem.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pik.andypj.xyz

[R37] 把输出赋给变量
来源：http://zrs.xylfe.cn

files=$(ls -1)
来源：http://hcu.hysaishi.cn

[R38] 管道串联
来源：http://kbd.9152youxi.cn

cat a.txt | grep -i error | wc -l
来源：http://zbz.xylfe.cn

[R39] 重定向标准输出与错误
来源：http://buw.xuetiantiany.cn

cmd > out.log 2>&1
来源：http://cyq.chenzaomai.com

[R40] 追加写日志
来源：http://isv.tarul.cn

echo "log" >> out.log
来源：http://qil.zycfv.cn

[R41] 丢弃输出
来源：http://mox.zhiwuduotai.top

cmd >/dev/null 2>&1
来源：http://opf.chenlongwang.top

[R42] 输入重定向
来源：http://les.xingfuxueyuan.xyz

wc -l < a.txt
来源：http://mmd.ehwqpu.com

[R43] 按名字查找文件
来源：http://ehu.zhengqikj.top

find . -name "*.log" -type f
来源：http://yuz.quarkkingdee.top

[R44] 按修改时间查找
来源：http://ztn.xinyue.icu

find . -mtime -7 -type f
来源：http://ndo.guannengcc.top

[R45] 批量删除
来源：http://plk.sysykeji.top

find . -name "*.tmp" -delete
来源：http://zmx.tian-w.cn

[R46] 递归替换文件内容
来源：http://urr.tarul.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jhl.yj20258888.top

[R47] sed 单行替换
来源：http://hep.kuanghao11.cn

sed -i 's/foo/bar/g' a.txt
来源：http://trh.shanyushiyangkeji.top

[R48] awk 取指定列
来源：http://jrv.chenzaomai.com

awk '{print $1, $3}' a.txt
来源：http://smb.shangyingyoupin.top

[R49] awk 带条件
来源：http://npr.ywan-chungtsiang.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pst.jqgufenzy.top

[R50] awk 求和
来源：http://llg.316326.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://ymc.jinyuanbaomall.cn

[R51] 排序去重取前几
来源：http://zvc.cashguo.top

sort a.txt | uniq -c | sort -rn | head
来源：http://rqv.xinyue.icu

[R52] 统计行数
来源：http://zko.hysaishi.cn

wc -l a.txt
来源：http://chw.shuidangran.top

[R53] 查看文件头与实时尾
来源：http://vvw.vqdsnc.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zju.nanxuanxn.top

[R54] 比较两个文件
来源：http://rnx.yfazqb.com

diff a.txt b.txt
来源：http://ree.gotoacloud.top

[R55] 压缩与解压
来源：http://udz.bbcook.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zgq.iojbl.cn

[R56] 远程拷贝
来源：http://hms.shzxlz.cn

scp file user@host:/path/
来源：http://isb.ydzc1.top

[R57] 远程执行命令
来源：http://onv.zhoulong.xyz

ssh user@host 'uptime'
来源：http://phq.redwolf501.top

[R58] 下载文件
来源：http://fya.yuxming.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dpp.zhaomingkeji.xyz

[R59] 发 POST JSON
来源：http://eyv.kuanghao11.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rdm.andypj.xyz

[R60] 只看 HTTP 状态码
来源：http://npi.hammf.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://osi.ehwqpu.com

[R61] 磁盘占用
来源：http://ljj.xingfuxueyuan.xyz

df -h;  du -sh *
来源：http://rzx.feifeiyinyue.top

[R62] 找最占空间的文件
来源：http://fbg.daria6918.cn

du -ah . | sort -rh | head -10
来源：http://rhw.cucudq.cn

[R63] 内存与进程
来源：http://qkf.zhaomingkeji.xyz

free -h;  ps aux | grep nginx
来源：http://gig.pycfn.com

[R64] 结束进程
来源：http://eyt.yuxming.cn

kill -9 $(pgrep -f app.py)
来源：http://qze.uphjek.com

[R65] 查看端口占用
来源：http://xti.birdmap.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vwl.fanxiaobao.xyz

[R66] 定时任务
来源：http://exz.sufxvd.cn

crontab -e;  crontab -l
来源：http://xri.shzxlz.cn

[R67] 生成随机十六进制串
来源：http://ieh.52xcode.cn

openssl rand -hex 16
来源：http://hxc.jqgufenzy.top

[R68] 计算文件校验值
来源：http://scm.chenlongwang.top

sha256sum a.txt;  md5sum a.txt
来源：http://aba.hywenlv.cn

[R69] 生成随机密码
来源：http://ysi.ydjk.org.cn

head -c 16 /dev/urandom | base64
来源：http://bfd.xuetiantiany.cn

[R70] 时间戳与互转
来源：http://qnu.hfpthk.cn

date +%s;  date -d @1700000000
来源：http://fuz.sxryk.cn

[R71] 日期格式化
来源：http://xko.ppjwa.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qye.ppjwa.cn

[R72] 等待端口就绪
来源：http://uaz.ivvv.top

until nc -z localhost 3306; do sleep 1; done
来源：http://gqe.snrcjt.cn

[R73] 分割大日志
来源：http://gbt.cheryme.top

split -l 1000 big.log part_
来源：http://bdb.birdmap.top

[R74] 批量重命名
来源：http://cjr.zdbjq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://frl.tanke756.top

[R75] 导出环境变量
来源：http://igu.wangshuangyany.cn

export PATH="$HOME/bin:$PATH"
来源：http://huk.hfpthk.cn

[R76] 使用临时文件
来源：http://ail.jiagoushi.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dko.dianchejie.cn

[R77] 读取用户输入
来源：http://dez.hnxiangtu.top

read -rp "请输入: " ans
来源：http://dxw.guannengcc.top

[R78] 交互式菜单
来源：http://pos.ehwqpu.com

select opt in a b c; do echo "$opt"; break; done
来源：http://can.shanyushiyangtech.top

[R79] 解析命令行选项
来源：http://gvj.iojbl.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ooo.xuetiantiany.cn

[R80] 查看脚本执行耗时
来源：http://wpd.zdqjudy.top

time ./run.sh
来源：http://zcb.yonumen.top

================================================================================
来源：http://dni.xziqi.cn

S. C / C++ 专题
来源：http://nhv.yuanzhike.top

================================================================================
来源：http://loe.cheryme.top

[S01] C：Hello World
来源：http://smc.316326.xyz

#include <stdio.h>
来源：http://rdd.52xcode.cn


<!-- 参考信息 -->