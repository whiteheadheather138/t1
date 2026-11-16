代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://njw.hcnkem.com

[Q32] 分组拼接字符串
来源：http://iqm.hysaishi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://igb.gaohongyu789.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rgv.yuxming.cn

[Q33] 多列分组
来源：http://oyi.gotoacloud.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ufq.ywan-chungtsiang.top

[Q34] 每组取第一条
来源：http://cxa.gzhubu.top

SELECT * FROM (
来源：http://toc.fzhhl.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xeu.smart0.xyz

) t WHERE rn = 1;
来源：http://nit.yj20258888.top

[Q35] 内连接
来源：http://cun.ehwqpu.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vvk.zhijiandao.cn

[Q36] 左连接
来源：http://liz.vqdsnc.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wyd.shzxlz.cn

[Q37] 右连接
来源：http://okr.shanyushiyangtech.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://udp.yuxming.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mrj.guowangkeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dtd.sxryk.cn

[Q39] 自连接（查上下级）
来源：http://wfr.jqgfzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://lcm.hnqzz.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hek.quarkkingdee.top

[Q40] 交叉连接（笛卡尔积）
来源：http://iao.zdqjudy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hqh.nanxinkj.top

[Q41] 多表连接
来源：http://yyl.bbcook.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ahq.fzhhl.top

JOIN users u ON u.id = o.user_id
来源：http://zcb.jyoumei.cn

JOIN products p ON p.id = o.product_id;
来源：http://jwk.hfpthk.cn

[Q42] 连接条件附加过滤
来源：http://uib.shangyingyoupin.top

SELECT u.name, o.amount FROM users u
来源：http://eek.gotoacloud.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vfl.daria6918.cn

[Q43] 标量子查询
来源：http://whq.cdnleiting.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ntp.kuanghao11.cn

[Q44] IN 子查询
来源：http://udy.vehdjk.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lce.xuanzx.com

[Q45] EXISTS 判断存在
来源：http://fph.xinyue.icu

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tal.yuxming.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hnb.dianchejie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eqc.zhijiandao.cn

[Q47] 与平均值比较
来源：http://ynh.xinyue.icu

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dyh.hcnkem.com

[Q48] CTE 公用表表达式
来源：http://pur.zhongyouzk.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dzq.jinqigufen.top

SELECT * FROM t WHERE c > 5;
来源：http://rth.feifeiyinyue.top

[Q49] 更新单行
来源：http://ftb.xuanzx.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vse.chenzaomai.com

[Q50] 批量更新
来源：http://vrq.fzhhl.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://odn.shuidangran.top

[Q51] 用子查询更新
来源：http://szc.birdmap.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ahx.haohaochexian.top

[Q52] 删除指定行
来源：http://kfp.xinyue.icu

DELETE FROM users WHERE id = 10;
来源：http://lwo.hnxiangtu.top

[Q53] 按条件删除
来源：http://ikg.fktsv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rku.gogol.net.cn

[Q54] 清空表
来源：http://fpu.daria6918.cn

TRUNCATE TABLE logs;
来源：http://lxj.quarkkingdee.top

[Q55] 排名（并列占位）
来源：http://tjp.pycfn.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wvx.fzhhl.top

[Q56] 密集排名（并列不占位）
来源：http://mes.gaohongyu789.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pdx.chenjidiqi.icu

[Q57] 行号
来源：http://ves.yvedp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uqc.nanxinkj.top

[Q58] 累计求和
来源：http://hct.ivvv.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://frn.fehbvm.com

[Q59] 分组内累计
来源：http://ksn.shanyushiyangkeji.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fel.yueranfly.top

[Q60] 取上一行 / 下一行
来源：http://dkr.hywenlv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zbp.pengpengdd.cyou

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hsp.wangshuangyany.cn

[Q61] 移动平均
来源：http://emq.jinyuanbaomall.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qzv.shanyushiyangkeji.top

[Q62] 分组占比
来源：http://rqz.yuanzhike.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ioz.cdnleiting.top

[Q63] 开启事务
来源：http://axl.chenlongwang.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ocm.ctjpmb.com

[Q64] 提交事务
来源：http://uql.xziqi.cn

COMMIT;
来源：http://cfm.havefunace.top

[Q65] 回滚事务
来源：http://dgg.hammf.cn

ROLLBACK;
来源：http://eau.zhengqikj.top

[Q66] 行锁查询
来源：http://ewq.yvedp.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vic.bjfxy.top

[Q67] 设置隔离级别
来源：http://xyi.ywan-chungtsiang.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sih.vehdjk.com

[Q68] 保存点
来源：http://eaz.hysaishi.cn

SAVEPOINT sp1;
来源：http://znt.hfpthk.cn

ROLLBACK TO sp1;
来源：http://cxv.chenlongwang.top

[Q69] 查看执行计划
来源：http://cgm.epnwcf.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nqb.cdnleiting.top

[Q70] 更新统计信息
来源：http://gcq.vehdjk.com

ANALYZE TABLE users;
来源：http://idc.guowangkeji.top

[Q71] 查看建表语句
来源：http://gpp.ybcxt.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ofe.gzhubu.top

[Q72] 查看索引
来源：http://kgj.ydzc1.top

SHOW INDEX FROM users;
来源：http://lea.quarkkingdee.top

[Q73] 查看表状态
来源：http://bhm.sysykeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ijz.svipenyu.cn

[Q74] 强制使用索引
来源：http://niq.yuanzhike.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lin.meibo888.top

[Q75] 日期格式化
来源：http://nwk.hesvh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://btz.fanxiaobao.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wfc.vqdsnc.cn

[Q76] 按天统计
来源：http://hor.zhengqikj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://edu.xziqi.cn

[Q77] 时间加减
来源：http://cxx.0kj1m.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eha.iojbl.cn

[Q78] 当前时间
来源：http://kdw.316326.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ctm.fengsongda.top

[Q79] 字符串拼接
来源：http://evl.uphjek.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xpo.fehbvm.com

[Q80] 字符串截取
来源：http://osz.shzxlz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rzh.sxryk.cn

[Q81] 字符串替换
来源：http://qeb.gzhubu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fvb.shuidangran.top

[Q82] 字符长度与字节长度
来源：http://zca.yueranfly.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hsk.316326.xyz

[Q83] 大小写转换
来源：http://ldb.hcnkem.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gnl.haohaochexian.top

[Q84] 去除首尾空格
来源：http://zjq.zdqjudy.top

SELECT TRIM(name) FROM users;
来源：http://kno.jqgufenzy.top

[Q85] 数值取整
来源：http://uko.chenlongwang.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vun.uphjek.com

[Q86] 读取 JSON 字段
来源：http://niz.nwbrower.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://btl.jqgfzy.top

[Q87] JSON 字段做条件
来源：http://rpq.ehwqpu.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nrr.hysaishi.cn

[Q88] 行转列（条件聚合）
来源：http://xmv.guowangkeji.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yna.yj202588.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ajq.bbcook.cn

[Q89] 判断表是否存在
来源：http://pso.zhaomingkeji.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://iex.pengpengdd.cyou

[Q90] 生成序号列
来源：http://hvv.zhiwuduotai.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mgw.yuxming.cn

================================================================================
来源：http://tra.jinqigfzy.top

R. Bash 专题
来源：http://ozo.tanke756.top

================================================================================
来源：http://udo.nwbrower.top

[R01] shebang 与严格模式
来源：http://env.fehbvm.com

#!/usr/bin/env bash
来源：http://yxm.fzhhl.top

set -euo pipefail
来源：http://lgv.gotoacloud.top

[R02] 变量赋值与使用
来源：http://ioj.yueranfly.top

name="Tom"; echo "$name"
来源：http://dnh.jinqigfzy.top

[R03] 只读变量
来源：http://smm.pycfn.com

readonly PI=3.14
来源：http://rzm.zhengqikj.top

[R04] 位置参数
来源：http://pgj.chenzaomai.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tjz.hnqzz.top

[R05] 参数默认值
来源：http://tpc.hongshengwenyu.top

name="${1:-default}"
来源：http://vld.shzxlz.cn

[R06] 判断命令是否存在
来源：http://wxf.sxryk.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lwb.gotoacloud.top

[R07] if 判断文件
来源：http://aii.yuanzhike.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nsk.zhaomingkeji.xyz

[R08] 数值比较
来源：http://zvl.hesvh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xwu.pycfn.com

[R09] 字符串比较
来源：http://nsj.shzxlz.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rsl.xuanzx.com

[R10] 正则匹配
来源：http://kni.hongshengwenyu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://eak.jinyuanbaomall.cn

[R11] case 多分支
来源：http://zjp.vehdjk.com

case "$1" in
来源：http://xof.yj202588.top

start) echo "启动" ;;
来源：http://yda.smart0.xyz

stop)  echo "停止" ;;
来源：http://nim.pycfn.com

*)     echo "未知命令" ;;
来源：http://dop.yfazqb.com

esac
来源：http://jso.xylfe.cn

[R12] for 遍历文件
来源：http://xhx.yanxiufei.cn

for f in *.txt; do echo "$f"; done
来源：http://ruw.yj20258888.top

[R13] for 计数循环
来源：http://vzn.yonumen.top

for i in {1..10}; do echo "$i"; done
来源：http://lra.yfazqb.com

[R14] C 风格 for
来源：http://kwd.cqqwz.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kgm.ctjpmb.com

[R15] while 逐行读文件
来源：http://omc.ivvv.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rvv.guannengcc.top

[R16] until 等待条件
来源：http://sgg.sxryk.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://piv.zycfv.cn

[R17] 数组定义与取值
来源：http://bsq.cqqwz.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wot.316326.xyz

[R18] 遍历数组
来源：http://scb.ehwqpu.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://unj.zycfv.cn

[R19] 数组长度
来源：http://apu.ydzc1.top

echo "${#arr[@]}"
来源：http://ero.cucudq.cn

[R20] 关联数组（字典）
来源：http://jsm.zhiwuduotai.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cbc.yuxming.cn

[R21] 字符串长度
来源：http://nru.zycfv.cn

echo "${#s}"
来源：http://fdu.yongpay.top

[R22] 截取子串
来源：http://uhl.yvedp.cn

echo "${s:0:5}"
来源：http://xzt.ywan-chungtsiang.top

[R23] 字符串替换
来源：http://fjh.daxiang520.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://isl.sufxvd.cn

[R24] 大小写转换
来源：http://ilo.chenjidiqi.icu

echo "${s^^}"; echo "${s,,}"
来源：http://fow.aibaodan.cn

[R25] 去后缀 / 去前缀
来源：http://vyt.jlsjyb.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xfm.gogol.net.cn

[R26] 命令替换
来源：http://raf.redwolf501.top

now=$(date +%F); echo "$now"
来源：http://pth.zhaomingkeji.xyz

[R27] 算术展开
来源：http://bea.xinyue.icu

echo $((1 + 2 * 3))
来源：http://vvi.fktsv.cn

[R28] 浮点运算
来源：http://sgb.hammf.cn

echo "scale=2; 10/3" | bc
来源：http://ryr.uphjek.com

[R29] 定义函数
来源：http://vho.xinyue.icu

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qby.yfazqb.com

[R30] 函数返回状态码
来源：http://usn.hcnkem.com

f() { return 0; }; f || echo "失败了"
来源：http://tit.sjlbkw.cn

[R31] 局部变量
来源：http://xte.yj202588.top

f() { local x=1; echo "$x"; }
来源：http://jks.tianlin.xyz

[R32] 参数个数校验
来源：http://ufw.feifeiyinyue.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tpv.iojbl.cn

[R33] 捕获错误并提示行号
来源：http://tyy.c1oappe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ttq.redwolf501.top

[R34] 退出时清理
来源：http://hly.yueranfly.top

trap 'rm -f "$tmp"' EXIT
来源：http://kvo.jianghu66.top

[R35] 后台执行并等待
来源：http://iyt.tarul.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pvw.tian-w.cn

[R36] 并发执行多个任务
来源：http://sbw.mhx1999.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rxc.gogol.net.cn

[R37] 把输出赋给变量
来源：http://yjf.zhijiandao.cn

files=$(ls -1)
来源：http://hah.hywenlv.cn

[R38] 管道串联
来源：http://qhn.hnxiangtu.top

cat a.txt | grep -i error | wc -l
来源：http://hih.zhengqikj.top

[R39] 重定向标准输出与错误
来源：http://bwi.yuanzhike.top

cmd > out.log 2>&1
来源：http://vho.hongshengwenyu.top

[R40] 追加写日志
来源：http://mhg.iojbl.cn

echo "log" >> out.log
来源：http://jge.gaohongyu789.top

[R41] 丢弃输出
来源：http://cmf.yj20258888.top

cmd >/dev/null 2>&1
来源：http://tdu.pengpengdd.cyou

[R42] 输入重定向
来源：http://rca.zhixingplan.top

wc -l < a.txt
来源：http://zfw.yuxming.cn

[R43] 按名字查找文件
来源：http://kxx.yueranfly.top

find . -name "*.log" -type f
来源：http://mgk.xinyue.icu

[R44] 按修改时间查找
来源：http://njf.aizwys.cn

find . -mtime -7 -type f
来源：http://bqu.zhixingplan.top

[R45] 批量删除
来源：http://vlw.yvedp.cn

find . -name "*.tmp" -delete
来源：http://fru.hesvh.cn

[R46] 递归替换文件内容
来源：http://ifc.fanxiaobao.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://idl.quarkkingdee.top

[R47] sed 单行替换
来源：http://twz.xuetiantiany.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qzd.mhx1999.top

[R48] awk 取指定列
来源：http://ewq.birdmap.top

awk '{print $1, $3}' a.txt
来源：http://zsi.vehdjk.com

[R49] awk 带条件
来源：http://pkv.c1oappe.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://njg.yanxiufei.cn

[R50] awk 求和
来源：http://yae.zhaomingkeji.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://tkq.dianchejie.cn

[R51] 排序去重取前几
来源：http://sge.chenjidiqi.icu

sort a.txt | uniq -c | sort -rn | head
来源：http://hoz.shanyushiyangkeji.top

[R52] 统计行数
来源：http://brk.sweek.top

wc -l a.txt
来源：http://oxf.chenlongwang.top

[R53] 查看文件头与实时尾
来源：http://dcs.quarkkingdee.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://aee.chenzaomai.com

[R54] 比较两个文件
来源：http://alj.wangdashe.top

diff a.txt b.txt
来源：http://vaf.yanxiufei.cn

[R55] 压缩与解压
来源：http://tvc.tian-w.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dcc.ydzc1.top

[R56] 远程拷贝
来源：http://ozq.hongshengwenyu.top

scp file user@host:/path/
来源：http://sbl.fengsongda.top

[R57] 远程执行命令
来源：http://nkr.havefunace.top

ssh user@host 'uptime'
来源：http://cme.jianghu66.top

[R58] 下载文件
来源：http://kur.xuetiantiany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fvw.kuanghao11.cn

[R59] 发 POST JSON
来源：http://pud.yj20258.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://isp.andypj.xyz

[R60] 只看 HTTP 状态码
来源：http://ems.xziqi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://noh.0kj1m.cn

[R61] 磁盘占用
来源：http://emo.zdbjq.cn

df -h;  du -sh *
来源：http://tti.shuidangran.top

[R62] 找最占空间的文件
来源：http://gls.haohaochexian.top

du -ah . | sort -rh | head -10
来源：http://ndq.yonumen.top

[R63] 内存与进程
来源：http://zvq.yuxming.cn

free -h;  ps aux | grep nginx
来源：http://agt.chenjidiqi.icu

[R64] 结束进程
来源：http://bjn.zycfv.cn

kill -9 $(pgrep -f app.py)
来源：http://wry.zhengqikj.top

[R65] 查看端口占用
来源：http://ebb.fengsongda.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lue.epnwcf.com

[R66] 定时任务
来源：http://vhf.hammf.cn

crontab -e;  crontab -l
来源：http://tfl.chenjidiqi.icu

[R67] 生成随机十六进制串
来源：http://beq.fktsv.cn

openssl rand -hex 16
来源：http://wyy.cqqwz.cn

[R68] 计算文件校验值
来源：http://ech.yj20258.top

sha256sum a.txt;  md5sum a.txt
来源：http://dyr.snrcjt.cn

[R69] 生成随机密码
来源：http://rdi.vqdsnc.cn

head -c 16 /dev/urandom | base64
来源：http://knn.kuanghao11.cn

[R70] 时间戳与互转
来源：http://znh.fengsongda.top

date +%s;  date -d @1700000000
来源：http://fti.daxiang520.top

[R71] 日期格式化
来源：http://blb.redwolf501.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://wfk.yongpay.top

[R72] 等待端口就绪
来源：http://egy.yueranfly.top

until nc -z localhost 3306; do sleep 1; done
来源：http://thl.ivvv.top

[R73] 分割大日志
来源：http://eyy.pengpengdd.cyou

split -l 1000 big.log part_
来源：http://zpj.haohaochexian.top

[R74] 批量重命名
来源：http://oug.yj202588.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bjr.tanke756.top

[R75] 导出环境变量
来源：http://qfa.fanxiaobao.xyz

export PATH="$HOME/bin:$PATH"
来源：http://iku.shangyingyoupin.top

[R76] 使用临时文件
来源：http://ccr.zhongyouzk.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jjc.nanxuanxn.top

[R77] 读取用户输入
来源：http://rlx.ehwqpu.com

read -rp "请输入: " ans
来源：http://bio.shuidangran.top

[R78] 交互式菜单
来源：http://bfb.fanxiaobao.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://gla.zhengqikj.top

[R79] 解析命令行选项
来源：http://ulp.tanke756.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ims.zhengqikj.top

[R80] 查看脚本执行耗时
来源：http://dzd.nanxinkj.top

time ./run.sh
来源：http://fxh.yj202588.top

================================================================================
来源：http://qba.shanyushiyangkeji.top


<!-- 参考信息 -->