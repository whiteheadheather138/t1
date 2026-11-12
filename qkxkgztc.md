代发 wailian999

[Q33] 多列分组
来源：http://ogd.fengsongda.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mtm.shanyushiyangkeji.top

[Q34] 每组取第一条
来源：http://fkl.bjfxy.top

SELECT * FROM (
来源：http://zfy.hnqzz.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gyp.chenjidiqi.icu

) t WHERE rn = 1;
来源：http://muk.quarkkingdee.top

[Q35] 内连接
来源：http://jbf.ppjwa.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bhd.shuidangran.top

[Q36] 左连接
来源：http://xfh.tarul.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ytn.pengpengdd.cyou

[Q37] 右连接
来源：http://wkm.redwolf501.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uxt.andypj.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://lvl.aizwys.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gxc.jqgfzy.top

[Q39] 自连接（查上下级）
来源：http://bud.pengpengdd.cyou

SELECT e.name, m.name AS manager FROM employees e
来源：http://cad.jinghuilouyu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rct.guannengcc.top

[Q40] 交叉连接（笛卡尔积）
来源：http://iiq.yongpay.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xno.xinyue.icu

[Q41] 多表连接
来源：http://nkh.feifeiyinyue.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://fcn.jlsjyb.cn

JOIN users u ON u.id = o.user_id
来源：http://hgz.wangshuangyany.cn

JOIN products p ON p.id = o.product_id;
来源：http://hxr.uphjek.com

[Q42] 连接条件附加过滤
来源：http://sfi.chenlongwang.top

SELECT u.name, o.amount FROM users u
来源：http://zek.feifeiyinyue.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zwj.chenzaomai.com

[Q43] 标量子查询
来源：http://exf.hfpthk.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://orb.zdbjq.cn

[Q44] IN 子查询
来源：http://xbf.wangdashe.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://peb.jqgufenzy.top

[Q45] EXISTS 判断存在
来源：http://inj.zhixingplan.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jkq.hesvh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fui.jianghu66.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gmc.nwbrower.top

[Q47] 与平均值比较
来源：http://tev.hysaishi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hpl.jinqigfzy.top

[Q48] CTE 公用表表达式
来源：http://rgi.jiagoushi.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gfs.hcnkem.com

SELECT * FROM t WHERE c > 5;
来源：http://nku.jinqigfzy.top

[Q49] 更新单行
来源：http://suq.haohaochexian.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ucz.cheryme.top

[Q50] 批量更新
来源：http://opt.pengpengdd.cyou

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zrg.haohaochexian.top

[Q51] 用子查询更新
来源：http://rqs.shangyingyoupin.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lts.shanyushiyangkeji.top

[Q52] 删除指定行
来源：http://ght.haohaochexian.top

DELETE FROM users WHERE id = 10;
来源：http://nfz.zdqjudy.top

[Q53] 按条件删除
来源：http://umw.shanyushiyangtech.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gau.zhoulong.xyz

[Q54] 清空表
来源：http://jeh.gogol.net.cn

TRUNCATE TABLE logs;
来源：http://nim.zdqjudy.top

[Q55] 排名（并列占位）
来源：http://gdd.mhx1999.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jie.guowangkeji.top

[Q56] 密集排名（并列不占位）
来源：http://ecf.0kj1m.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lhk.iojbl.cn

[Q57] 行号
来源：http://ajf.xuanzx.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bqd.tian-w.cn

[Q58] 累计求和
来源：http://yij.yongpay.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rqi.ehwqpu.com

[Q59] 分组内累计
来源：http://djf.ivvv.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://eiv.fktsv.cn

[Q60] 取上一行 / 下一行
来源：http://sxm.gzhubu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lua.fengsongda.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://iqa.yfazqb.com

[Q61] 移动平均
来源：http://dxe.shanyushiyangkeji.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://aqo.bbcook.cn

[Q62] 分组占比
来源：http://aqq.yj20258.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pha.yueranfly.top

[Q63] 开启事务
来源：http://owz.shanyushiyangtech.top

START TRANSACTION;                -- 或 BEGIN
来源：http://vdt.jinyuanbaomall.cn

[Q64] 提交事务
来源：http://xjr.yongpay.top

COMMIT;
来源：http://vha.vqdsnc.cn

[Q65] 回滚事务
来源：http://nnh.yueranfly.top

ROLLBACK;
来源：http://pip.sxryk.cn

[Q66] 行锁查询
来源：http://xly.fzhhl.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fsf.zycfv.cn

[Q67] 设置隔离级别
来源：http://oll.fehbvm.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://thq.hnqzz.top

[Q68] 保存点
来源：http://sdr.gogol.net.cn

SAVEPOINT sp1;
来源：http://ilh.hnqzz.top

ROLLBACK TO sp1;
来源：http://juj.jyoumei.cn

[Q69] 查看执行计划
来源：http://qrg.xinyue.icu

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yem.dashuyun.cn

[Q70] 更新统计信息
来源：http://epr.0kj1m.cn

ANALYZE TABLE users;
来源：http://gle.hfpthk.cn

[Q71] 查看建表语句
来源：http://nsj.hnqzz.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ldg.ehwqpu.com

[Q72] 查看索引
来源：http://zwp.pengpengdd.cyou

SHOW INDEX FROM users;
来源：http://kof.quarkkingdee.top

[Q73] 查看表状态
来源：http://sgt.fengsongda.top

SHOW TABLE STATUS LIKE 'users';
来源：http://sfn.meibo888.top

[Q74] 强制使用索引
来源：http://apr.yangfankeji.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://arv.hysaishi.cn

[Q75] 日期格式化
来源：http://prv.shanyushiyangtech.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vqn.jinqigfzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ndk.yj20258.top

[Q76] 按天统计
来源：http://gon.ivvv.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fat.cheryme.top

[Q77] 时间加减
来源：http://hvw.feifeiyinyue.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://leb.dianchejie.cn

[Q78] 当前时间
来源：http://lds.jinqigufen.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vfm.guannengcc.top

[Q79] 字符串拼接
来源：http://xow.nanxuanxn.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://twk.yonumen.top

[Q80] 字符串截取
来源：http://nni.hnxiangtu.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nbf.dianchejie.cn

[Q81] 字符串替换
来源：http://ahe.jiagoushi.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lpe.yanxiufei.cn

[Q82] 字符长度与字节长度
来源：http://xsq.sweek.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qzy.mhx1999.top

[Q83] 大小写转换
来源：http://omi.sxryk.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lrc.zycfv.cn

[Q84] 去除首尾空格
来源：http://yku.xingfuxueyuan.xyz

SELECT TRIM(name) FROM users;
来源：http://nzk.snrcjt.cn

[Q85] 数值取整
来源：http://qwf.gogol.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ssd.gaohongyu789.top

[Q86] 读取 JSON 字段
来源：http://sjh.hfpthk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ole.nanxuanxn.top

[Q87] JSON 字段做条件
来源：http://ydx.hnxiangtu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fsw.xuetiantiany.cn

[Q88] 行转列（条件聚合）
来源：http://jse.gaohongyu789.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xch.hesvh.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yjk.meibo888.top

[Q89] 判断表是否存在
来源：http://hvz.cucudq.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dli.yonumen.top

[Q90] 生成序号列
来源：http://lvs.nanxinkj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wmv.vqdsnc.cn

================================================================================
来源：http://xjr.sysykeji.top

R. Bash 专题
来源：http://smj.shanyushiyangtech.top

================================================================================
来源：http://bfr.shzxlz.cn

[R01] shebang 与严格模式
来源：http://rbk.c1oappe.top

#!/usr/bin/env bash
来源：http://npc.xuetiantiany.cn

set -euo pipefail
来源：http://tmj.gzhubu.top

[R02] 变量赋值与使用
来源：http://dkl.ywan-chungtsiang.top

name="Tom"; echo "$name"
来源：http://gvt.ydjk.org.cn

[R03] 只读变量
来源：http://jux.fanxiaobao.xyz

readonly PI=3.14
来源：http://wsl.ivvv.top

[R04] 位置参数
来源：http://eym.wangshuangyany.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mtx.zhiwuduotai.top

[R05] 参数默认值
来源：http://vyy.yangfankeji.com

name="${1:-default}"
来源：http://amt.jianghu66.top

[R06] 判断命令是否存在
来源：http://fgx.gotoacloud.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rst.dashuyun.cn

[R07] if 判断文件
来源：http://cdg.zdbjq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yjj.aizwys.cn

[R08] 数值比较
来源：http://nhr.52xcode.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ogn.cucudq.cn

[R09] 字符串比较
来源：http://tvu.shanyushiyangtech.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wzi.yonumen.top

[R10] 正则匹配
来源：http://ebe.52xcode.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tlm.feifeiyinyue.top

[R11] case 多分支
来源：http://mqc.aibaodan.cn

case "$1" in
来源：http://ssk.yuxming.cn

start) echo "启动" ;;
来源：http://ont.jqgufenzy.top

stop)  echo "停止" ;;
来源：http://vrq.9152youxi.cn

*)     echo "未知命令" ;;
来源：http://wvq.fzhhl.top

esac
来源：http://lsy.zhiwuduotai.top

[R12] for 遍历文件
来源：http://bei.yfazqb.com

for f in *.txt; do echo "$f"; done
来源：http://aga.ehwqpu.com

[R13] for 计数循环
来源：http://kmq.xinyue.icu

for i in {1..10}; do echo "$i"; done
来源：http://cil.zhengqikj.top

[R14] C 风格 for
来源：http://wtj.hcnkem.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fbp.quarkkingdee.top

[R15] while 逐行读文件
来源：http://iel.haohaochexian.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lai.jinyuanbaomall.cn

[R16] until 等待条件
来源：http://qmy.sysykeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vma.ivvv.top

[R17] 数组定义与取值
来源：http://ddb.uphjek.com

arr=(a b c); echo "${arr[0]}"
来源：http://wwu.tian-w.cn

[R18] 遍历数组
来源：http://ect.xziqi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xsw.zhongyouzk.top

[R19] 数组长度
来源：http://fbi.jinghuilouyu.cn

echo "${#arr[@]}"
来源：http://fvy.xuetiantiany.cn

[R20] 关联数组（字典）
来源：http://sed.hongshengwenyu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ixq.gogol.net.cn

[R21] 字符串长度
来源：http://dpr.jinqigfzy.top

echo "${#s}"
来源：http://yqx.xinyue.icu

[R22] 截取子串
来源：http://edc.yueranfly.top

echo "${s:0:5}"
来源：http://ziu.jiagoushi.top

[R23] 字符串替换
来源：http://izd.nanxuanxn.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vbg.ivvv.top

[R24] 大小写转换
来源：http://mnj.jlsjyb.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mbz.wangdashe.top

[R25] 去后缀 / 去前缀
来源：http://knk.jqgfzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://pyi.snrcjt.cn

[R26] 命令替换
来源：http://dph.ivvv.top

now=$(date +%F); echo "$now"
来源：http://thg.vehdjk.com

[R27] 算术展开
来源：http://lta.zhiwuduotai.top

echo $((1 + 2 * 3))
来源：http://ozv.ywan-chungtsiang.top

[R28] 浮点运算
来源：http://cyj.sysykeji.top

echo "scale=2; 10/3" | bc
来源：http://ukn.chenlongwang.top

[R29] 定义函数
来源：http://rcq.xuanzx.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wan.tarul.cn

[R30] 函数返回状态码
来源：http://cow.yuxming.cn

f() { return 0; }; f || echo "失败了"
来源：http://ugh.hammf.cn

[R31] 局部变量
来源：http://ewg.fehbvm.com

f() { local x=1; echo "$x"; }
来源：http://jsc.52xcode.cn

[R32] 参数个数校验
来源：http://kpv.0kj1m.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nhu.tarul.cn

[R33] 捕获错误并提示行号
来源：http://zko.wangdashe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://msg.xylfe.cn

[R34] 退出时清理
来源：http://kss.ybcxt.top

trap 'rm -f "$tmp"' EXIT
来源：http://wlz.shuidangran.top

[R35] 后台执行并等待
来源：http://ndh.haohaochexian.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xhs.yanxiufei.cn

[R36] 并发执行多个任务
来源：http://syv.gogol.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://phy.yanxiufei.cn

[R37] 把输出赋给变量
来源：http://rwu.cdnleiting.top

files=$(ls -1)
来源：http://qvs.hywenlv.cn

[R38] 管道串联
来源：http://egp.meibo888.top

cat a.txt | grep -i error | wc -l
来源：http://iid.fengsongda.top

[R39] 重定向标准输出与错误
来源：http://mww.jlsjyb.cn

cmd > out.log 2>&1
来源：http://mcm.hnqzz.top

[R40] 追加写日志
来源：http://mjt.dianchejie.cn

echo "log" >> out.log
来源：http://bwy.cheryme.top

[R41] 丢弃输出
来源：http://osf.gogol.net.cn

cmd >/dev/null 2>&1
来源：http://han.yuxming.cn

[R42] 输入重定向
来源：http://bfz.haohaochexian.top

wc -l < a.txt
来源：http://mpz.zdbjq.cn

[R43] 按名字查找文件
来源：http://kpr.aizwys.cn

find . -name "*.log" -type f
来源：http://zza.jlsjyb.cn

[R44] 按修改时间查找
来源：http://bre.cashguo.top

find . -mtime -7 -type f
来源：http://teh.ivvv.top

[R45] 批量删除
来源：http://wez.fktsv.cn

find . -name "*.tmp" -delete
来源：http://dgd.hnqzz.top

[R46] 递归替换文件内容
来源：http://fst.ppjwa.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iyh.hesvh.cn

[R47] sed 单行替换
来源：http://cgd.jianghu66.top

sed -i 's/foo/bar/g' a.txt
来源：http://kco.shangyingyoupin.top

[R48] awk 取指定列
来源：http://hht.cucudq.cn

awk '{print $1, $3}' a.txt
来源：http://wlr.nwbrower.top

[R49] awk 带条件
来源：http://ats.jlsjyb.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hhc.quarkkingdee.top

[R50] awk 求和
来源：http://ein.jinqigufen.top

awk '{s += $2} END {print s}' a.txt
来源：http://ykk.mhx1999.top

[R51] 排序去重取前几
来源：http://mja.jqgfzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ugu.gotoacloud.top

[R52] 统计行数
来源：http://ezz.daxiang520.top

wc -l a.txt
来源：http://qwl.aibaodan.cn

[R53] 查看文件头与实时尾
来源：http://wwo.jinyuanbaomall.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jqt.chenzaomai.com

[R54] 比较两个文件
来源：http://ave.bjfxy.top

diff a.txt b.txt
来源：http://cnw.epnwcf.com

[R55] 压缩与解压
来源：http://lzp.pycfn.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://szn.jlsjyb.cn

[R56] 远程拷贝
来源：http://wvg.316326.xyz

scp file user@host:/path/
来源：http://xtp.pengpengdd.cyou

[R57] 远程执行命令
来源：http://bny.pengpengdd.cyou

ssh user@host 'uptime'
来源：http://ipc.ctjpmb.com

[R58] 下载文件
来源：http://jom.vqdsnc.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xks.cdnleiting.top

[R59] 发 POST JSON
来源：http://wyi.ctjpmb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xex.jinqigufen.top

[R60] 只看 HTTP 状态码
来源：http://tgl.smart0.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rta.c1oappe.top

[R61] 磁盘占用
来源：http://spp.fktsv.cn

df -h;  du -sh *
来源：http://hws.0kj1m.cn

[R62] 找最占空间的文件
来源：http://xbd.316326.xyz

du -ah . | sort -rh | head -10
来源：http://mqx.jqgufenzy.top

[R63] 内存与进程
来源：http://xeu.tarul.cn

free -h;  ps aux | grep nginx
来源：http://yan.svipenyu.cn

[R64] 结束进程
来源：http://usq.kuanghao11.cn

kill -9 $(pgrep -f app.py)
来源：http://hwz.jlsjyb.cn

[R65] 查看端口占用
来源：http://vdf.xylfe.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pej.fktsv.cn

[R66] 定时任务
来源：http://gnj.xuanzx.com

crontab -e;  crontab -l
来源：http://hem.fehbvm.com

[R67] 生成随机十六进制串
来源：http://qjb.quarkkingdee.top

openssl rand -hex 16
来源：http://dhq.fanxiaobao.xyz

[R68] 计算文件校验值
来源：http://ggo.birdmap.top

sha256sum a.txt;  md5sum a.txt
来源：http://kvp.ehwqpu.com

[R69] 生成随机密码
来源：http://scd.cheryme.top

head -c 16 /dev/urandom | base64
来源：http://ysg.shuidangran.top

[R70] 时间戳与互转
来源：http://oqe.wangdashe.top

date +%s;  date -d @1700000000
来源：http://lhx.shanyushiyangtech.top

[R71] 日期格式化
来源：http://bpd.hywenlv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qjc.yangfankeji.com

[R72] 等待端口就绪
来源：http://hcj.fzhhl.top

until nc -z localhost 3306; do sleep 1; done
来源：http://duw.9152youxi.cn

[R73] 分割大日志
来源：http://stc.wangdashe.top

split -l 1000 big.log part_
来源：http://dyr.sufxvd.cn

[R74] 批量重命名
来源：http://wwp.gzhubu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://trj.haohaochexian.top

[R75] 导出环境变量
来源：http://rns.ydjk.org.cn

export PATH="$HOME/bin:$PATH"
来源：http://xoh.xingfuxueyuan.xyz

[R76] 使用临时文件
来源：http://slo.hammf.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zcc.meibo888.top

[R77] 读取用户输入
来源：http://jec.zhoulong.xyz

read -rp "请输入: " ans
来源：http://tlr.zhixingplan.top

[R78] 交互式菜单
来源：http://xdr.nwbrower.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ydc.ydzc1.top

[R79] 解析命令行选项
来源：http://dhx.xylfe.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ztm.9152youxi.cn

[R80] 查看脚本执行耗时
来源：http://lot.yj202588.top

time ./run.sh
来源：http://hhr.jqgufenzy.top

================================================================================
来源：http://hsh.cdnleiting.top

S. C / C++ 专题
来源：http://uuq.zhoulong.xyz

================================================================================
来源：http://jrn.xinyue.icu

[S01] C：Hello World
来源：http://pco.vqdsnc.cn

#include <stdio.h>
来源：http://ukb.bbcook.cn


<!-- 参考信息 -->