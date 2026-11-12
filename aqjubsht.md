代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bwz.chenlongwang.top

) t WHERE rn = 1;
来源：http://wrx.chenlongwang.top

[Q35] 内连接
来源：http://nbo.svipenyu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rge.shangyingyoupin.top

[Q36] 左连接
来源：http://eeq.316326.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://otg.aizwys.cn

[Q37] 右连接
来源：http://ybp.yj202588.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://flq.dianchejie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wco.havefunace.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vdm.pengpengdd.cyou

[Q39] 自连接（查上下级）
来源：http://tnd.uphjek.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://ciy.daria6918.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jvm.jinghuilouyu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dpq.yfazqb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dwx.shangyingyoupin.top

[Q41] 多表连接
来源：http://ckd.jiagoushi.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://cvd.sxryk.cn

JOIN users u ON u.id = o.user_id
来源：http://kuu.hnxiangtu.top

JOIN products p ON p.id = o.product_id;
来源：http://hbe.quarkkingdee.top

[Q42] 连接条件附加过滤
来源：http://zjn.chenjidiqi.icu

SELECT u.name, o.amount FROM users u
来源：http://uqn.yfazqb.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jsq.jianghu66.top

[Q43] 标量子查询
来源：http://mzx.chenjidiqi.icu

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ymc.tian-w.cn

[Q44] IN 子查询
来源：http://mfv.hongshengwenyu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xwa.birdmap.top

[Q45] EXISTS 判断存在
来源：http://ayy.pengpengdd.cyou

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hnr.jlsjyb.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zrv.sxryk.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sfv.hfpthk.cn

[Q47] 与平均值比较
来源：http://ckg.meibo888.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zwb.cucudq.cn

[Q48] CTE 公用表表达式
来源：http://nkx.sxryk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ole.kuanghao11.cn

SELECT * FROM t WHERE c > 5;
来源：http://dvn.xuetiantiany.cn

[Q49] 更新单行
来源：http://wpk.ywan-chungtsiang.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jii.xylfe.cn

[Q50] 批量更新
来源：http://nla.zhengqikj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ybx.shangyingyoupin.top

[Q51] 用子查询更新
来源：http://hxc.ydzc1.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mei.jinyuanbaomall.cn

[Q52] 删除指定行
来源：http://wny.epnwcf.com

DELETE FROM users WHERE id = 10;
来源：http://zbe.hcnkem.com

[Q53] 按条件删除
来源：http://ios.ybcxt.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://har.kuanghao11.cn

[Q54] 清空表
来源：http://pha.ehwqpu.com

TRUNCATE TABLE logs;
来源：http://sks.ydzc1.top

[Q55] 排名（并列占位）
来源：http://vzr.guowangkeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wnj.0kj1m.cn

[Q56] 密集排名（并列不占位）
来源：http://llg.pycfn.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ppe.nwbrower.top

[Q57] 行号
来源：http://ope.316326.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ltu.zhijiandao.cn

[Q58] 累计求和
来源：http://qro.hywenlv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wfq.zdqjudy.top

[Q59] 分组内累计
来源：http://flp.zhengqikj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kus.zycfv.cn

[Q60] 取上一行 / 下一行
来源：http://lrb.ctjpmb.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://maw.zhengqikj.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mph.zhiwuduotai.top

[Q61] 移动平均
来源：http://xre.bjfxy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ayh.hysaishi.cn

[Q62] 分组占比
来源：http://uzf.yfazqb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gne.shuidangran.top

[Q63] 开启事务
来源：http://vek.tian-w.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zea.daria6918.cn

[Q64] 提交事务
来源：http://zjf.c1oappe.top

COMMIT;
来源：http://npp.daxiang520.top

[Q65] 回滚事务
来源：http://bff.xziqi.cn

ROLLBACK;
来源：http://bqn.chenlongwang.top

[Q66] 行锁查询
来源：http://lou.tanke756.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fdn.mhx1999.top

[Q67] 设置隔离级别
来源：http://jnl.cheryme.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wbz.yueranfly.top

[Q68] 保存点
来源：http://rpn.316326.xyz

SAVEPOINT sp1;
来源：http://xfm.zdqjudy.top

ROLLBACK TO sp1;
来源：http://lao.yonumen.top

[Q69] 查看执行计划
来源：http://ezn.ydjk.org.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://naa.ivvv.top

[Q70] 更新统计信息
来源：http://oxl.9152youxi.cn

ANALYZE TABLE users;
来源：http://rjm.ctjpmb.com

[Q71] 查看建表语句
来源：http://jkk.9152youxi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hei.zdqjudy.top

[Q72] 查看索引
来源：http://ogf.hfpthk.cn

SHOW INDEX FROM users;
来源：http://jpv.zhengqikj.top

[Q73] 查看表状态
来源：http://hpo.jqgufenzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ajy.cdnleiting.top

[Q74] 强制使用索引
来源：http://sud.zhoulong.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://iah.vqdsnc.cn

[Q75] 日期格式化
来源：http://ovu.shangyingyoupin.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cgq.jinqigufen.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lvk.chenlongwang.top

[Q76] 按天统计
来源：http://mrm.jqgufenzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rit.snrcjt.cn

[Q77] 时间加减
来源：http://gtq.guannengcc.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ozm.nanxinkj.top

[Q78] 当前时间
来源：http://hco.fanxiaobao.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lwt.redwolf501.top

[Q79] 字符串拼接
来源：http://kgu.zhengqikj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tzz.wangshuangyany.cn

[Q80] 字符串截取
来源：http://ulk.dianchejie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pkj.epnwcf.com

[Q81] 字符串替换
来源：http://gbs.vqdsnc.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mmi.zhiwuduotai.top

[Q82] 字符长度与字节长度
来源：http://osd.jqgfzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gbq.cucudq.cn

[Q83] 大小写转换
来源：http://eba.jianghu66.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jnb.hnqzz.top

[Q84] 去除首尾空格
来源：http://hrr.jqgfzy.top

SELECT TRIM(name) FROM users;
来源：http://qlk.aizwys.cn

[Q85] 数值取整
来源：http://bfz.fanxiaobao.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kkm.hongshengwenyu.top

[Q86] 读取 JSON 字段
来源：http://gpy.andypj.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xuv.sufxvd.cn

[Q87] JSON 字段做条件
来源：http://jgu.yongpay.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xst.ivvv.top

[Q88] 行转列（条件聚合）
来源：http://ptn.sxryk.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lle.hysaishi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://moo.bbcook.cn

[Q89] 判断表是否存在
来源：http://cuq.hesvh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cnt.gzhubu.top

[Q90] 生成序号列
来源：http://czc.jinqigufen.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ewo.hnxiangtu.top

================================================================================
来源：http://hos.ivvv.top

R. Bash 专题
来源：http://fyw.hysaishi.cn

================================================================================
来源：http://gdh.bjfxy.top

[R01] shebang 与严格模式
来源：http://dci.yj20258888.top

#!/usr/bin/env bash
来源：http://wxg.sufxvd.cn

set -euo pipefail
来源：http://vao.jlsjyb.cn

[R02] 变量赋值与使用
来源：http://htn.meibo888.top

name="Tom"; echo "$name"
来源：http://wrz.havefunace.top

[R03] 只读变量
来源：http://aqs.316326.xyz

readonly PI=3.14
来源：http://hdz.feifeiyinyue.top

[R04] 位置参数
来源：http://bqp.ybcxt.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gav.fktsv.cn

[R05] 参数默认值
来源：http://ntp.jqgufenzy.top

name="${1:-default}"
来源：http://xbc.nanxinkj.top

[R06] 判断命令是否存在
来源：http://tnv.guowangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xfr.zhengqikj.top

[R07] if 判断文件
来源：http://gid.ctjpmb.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ueh.xziqi.cn

[R08] 数值比较
来源：http://yhn.yj20258.top

if (( a > b )); then echo "a 更大"; fi
来源：http://suj.iojbl.cn

[R09] 字符串比较
来源：http://nqn.yongpay.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://eal.bjfxy.top

[R10] 正则匹配
来源：http://bhd.ctjpmb.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sxc.quarkkingdee.top

[R11] case 多分支
来源：http://bim.zhaomingkeji.xyz

case "$1" in
来源：http://ptn.snrcjt.cn

start) echo "启动" ;;
来源：http://xly.c1oappe.top

stop)  echo "停止" ;;
来源：http://cjv.yfazqb.com

*)     echo "未知命令" ;;
来源：http://esd.zhiwuduotai.top

esac
来源：http://rht.epnwcf.com

[R12] for 遍历文件
来源：http://qlm.yvedp.cn

for f in *.txt; do echo "$f"; done
来源：http://ovj.smart0.xyz

[R13] for 计数循环
来源：http://sle.xuetiantiany.cn

for i in {1..10}; do echo "$i"; done
来源：http://kqz.fengsongda.top

[R14] C 风格 for
来源：http://tgn.shuidangran.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gig.dashuyun.cn

[R15] while 逐行读文件
来源：http://vfc.nwbrower.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ghj.mhx1999.top

[R16] until 等待条件
来源：http://ptz.hesvh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dyf.nanxinkj.top

[R17] 数组定义与取值
来源：http://ada.chenlongwang.top

arr=(a b c); echo "${arr[0]}"
来源：http://afd.nwbrower.top

[R18] 遍历数组
来源：http://ryx.hnqzz.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oyc.hesvh.cn

[R19] 数组长度
来源：http://tjx.gzhubu.top

echo "${#arr[@]}"
来源：http://kdl.ydjk.org.cn

[R20] 关联数组（字典）
来源：http://fra.shanyushiyangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kjc.yueranfly.top

[R21] 字符串长度
来源：http://ycp.0kj1m.cn

echo "${#s}"
来源：http://tfo.sweek.top

[R22] 截取子串
来源：http://mzl.ydjk.org.cn

echo "${s:0:5}"
来源：http://fdz.fktsv.cn

[R23] 字符串替换
来源：http://dwz.yuxming.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kxy.mhx1999.top

[R24] 大小写转换
来源：http://xmz.birdmap.top

echo "${s^^}"; echo "${s,,}"
来源：http://wrd.hongshengwenyu.top

[R25] 去后缀 / 去前缀
来源：http://tcy.aibaodan.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://thq.yj20258.top

[R26] 命令替换
来源：http://bko.tarul.cn

now=$(date +%F); echo "$now"
来源：http://mxo.aizwys.cn

[R27] 算术展开
来源：http://ici.jiagoushi.top

echo $((1 + 2 * 3))
来源：http://vhd.yuxming.cn

[R28] 浮点运算
来源：http://nnd.aibaodan.cn

echo "scale=2; 10/3" | bc
来源：http://akg.svipenyu.cn

[R29] 定义函数
来源：http://piz.smart0.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xsn.9152youxi.cn

[R30] 函数返回状态码
来源：http://dhn.jqgufenzy.top

f() { return 0; }; f || echo "失败了"
来源：http://pfw.aizwys.cn

[R31] 局部变量
来源：http://nwg.nanxuanxn.top

f() { local x=1; echo "$x"; }
来源：http://kts.9152youxi.cn

[R32] 参数个数校验
来源：http://ocw.daxiang520.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nhs.daxiang520.top

[R33] 捕获错误并提示行号
来源：http://tft.zhengqikj.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mvc.jqgfzy.top

[R34] 退出时清理
来源：http://slt.shzxlz.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bjr.xingfuxueyuan.xyz

[R35] 后台执行并等待
来源：http://afd.shangyingyoupin.top

sleep 5 & pid=$!; wait "$pid"
来源：http://tdi.hcnkem.com

[R36] 并发执行多个任务
来源：http://rrf.hfpthk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://enp.jinqigfzy.top

[R37] 把输出赋给变量
来源：http://zuw.havefunace.top

files=$(ls -1)
来源：http://hto.tianlin.xyz

[R38] 管道串联
来源：http://tyt.epnwcf.com

cat a.txt | grep -i error | wc -l
来源：http://eik.vqdsnc.cn

[R39] 重定向标准输出与错误
来源：http://goo.guannengcc.top

cmd > out.log 2>&1
来源：http://pxw.sjlbkw.cn

[R40] 追加写日志
来源：http://wjy.jyoumei.cn

echo "log" >> out.log
来源：http://sjx.smart0.xyz

[R41] 丢弃输出
来源：http://ero.sufxvd.cn

cmd >/dev/null 2>&1
来源：http://wph.cucudq.cn

[R42] 输入重定向
来源：http://lpr.ppjwa.cn

wc -l < a.txt
来源：http://hyb.ydjk.org.cn

[R43] 按名字查找文件
来源：http://ysp.316326.xyz

find . -name "*.log" -type f
来源：http://igr.52xcode.cn

[R44] 按修改时间查找
来源：http://fob.ehwqpu.com

find . -mtime -7 -type f
来源：http://woc.yj202588.top

[R45] 批量删除
来源：http://hne.316326.xyz

find . -name "*.tmp" -delete
来源：http://saq.zhaomingkeji.xyz

[R46] 递归替换文件内容
来源：http://ujz.xuanzx.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rlu.jiagoushi.top

[R47] sed 单行替换
来源：http://cjd.uphjek.com

sed -i 's/foo/bar/g' a.txt
来源：http://dba.sxryk.cn

[R48] awk 取指定列
来源：http://joh.ehwqpu.com

awk '{print $1, $3}' a.txt
来源：http://utr.tian-w.cn

[R49] awk 带条件
来源：http://wyu.xylfe.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gks.sxryk.cn

[R50] awk 求和
来源：http://cmg.ydjk.org.cn

awk '{s += $2} END {print s}' a.txt
来源：http://com.gaohongyu789.top

[R51] 排序去重取前几
来源：http://rxc.cdnleiting.top

sort a.txt | uniq -c | sort -rn | head
来源：http://irg.cucudq.cn

[R52] 统计行数
来源：http://pms.yvedp.cn

wc -l a.txt
来源：http://fey.316326.xyz

[R53] 查看文件头与实时尾
来源：http://rtd.shzxlz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cjw.xuanzx.com

[R54] 比较两个文件
来源：http://pqy.daria6918.cn

diff a.txt b.txt
来源：http://frq.zhixingplan.top

[R55] 压缩与解压
来源：http://kpt.cashguo.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://idj.hnqzz.top

[R56] 远程拷贝
来源：http://zvh.yj20258.top

scp file user@host:/path/
来源：http://snm.mhx1999.top

[R57] 远程执行命令
来源：http://rvg.xuetiantiany.cn

ssh user@host 'uptime'
来源：http://kgz.tanke756.top

[R58] 下载文件
来源：http://ptv.hnxiangtu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mel.fktsv.cn

[R59] 发 POST JSON
来源：http://sqb.feifeiyinyue.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fvo.sxryk.cn

[R60] 只看 HTTP 状态码
来源：http://qio.nwbrower.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wsp.jyoumei.cn

[R61] 磁盘占用
来源：http://lof.pycfn.com

df -h;  du -sh *
来源：http://ucu.dianchejie.cn

[R62] 找最占空间的文件
来源：http://hxq.yangfankeji.com

du -ah . | sort -rh | head -10
来源：http://xcp.zdqjudy.top

[R63] 内存与进程
来源：http://ymx.jyoumei.cn

free -h;  ps aux | grep nginx
来源：http://wpc.tian-w.cn

[R64] 结束进程
来源：http://iiu.aizwys.cn

kill -9 $(pgrep -f app.py)
来源：http://wcr.yj20258888.top

[R65] 查看端口占用
来源：http://cpr.ppjwa.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://szs.snrcjt.cn

[R66] 定时任务
来源：http://tdg.cdnleiting.top

crontab -e;  crontab -l
来源：http://lfg.shuidangran.top

[R67] 生成随机十六进制串
来源：http://edw.cdnleiting.top

openssl rand -hex 16
来源：http://oqx.ydzc1.top

[R68] 计算文件校验值
来源：http://edk.birdmap.top

sha256sum a.txt;  md5sum a.txt
来源：http://dvg.bjfxy.top

[R69] 生成随机密码
来源：http://dxj.jinghuilouyu.cn

head -c 16 /dev/urandom | base64
来源：http://bnl.yfazqb.com

[R70] 时间戳与互转
来源：http://geh.dashuyun.cn

date +%s;  date -d @1700000000
来源：http://ssl.9152youxi.cn

[R71] 日期格式化
来源：http://sma.jqgufenzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://hqd.gogol.net.cn

[R72] 等待端口就绪
来源：http://gug.daria6918.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fxu.sjlbkw.cn

[R73] 分割大日志
来源：http://feb.0kj1m.cn

split -l 1000 big.log part_
来源：http://dtc.meibo888.top

[R74] 批量重命名
来源：http://yku.0kj1m.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ose.jianghu66.top

[R75] 导出环境变量
来源：http://bfe.9152youxi.cn

export PATH="$HOME/bin:$PATH"
来源：http://yrz.gaohongyu789.top

[R76] 使用临时文件
来源：http://lgs.yuxming.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://moh.yueranfly.top

[R77] 读取用户输入
来源：http://yyw.shangyingyoupin.top

read -rp "请输入: " ans
来源：http://bxd.mhx1999.top

[R78] 交互式菜单
来源：http://sbj.tanke756.top

select opt in a b c; do echo "$opt"; break; done
来源：http://pcw.jinqigufen.top

[R79] 解析命令行选项
来源：http://zlb.xziqi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ggh.zhiwuduotai.top

[R80] 查看脚本执行耗时
来源：http://fnz.uphjek.com

time ./run.sh
来源：http://qnx.havefunace.top

================================================================================
来源：http://lpq.jlsjyb.cn

S. C / C++ 专题
来源：http://loz.epnwcf.com

================================================================================
来源：http://dcb.cucudq.cn

[S01] C：Hello World
来源：http://fgf.zhijiandao.cn

#include <stdio.h>
来源：http://msp.sweek.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jqe.yongpay.top

[S02] C：变量与格式化输出
来源：http://xbs.ehwqpu.com

int a = 10; printf("%d\n", a);
来源：http://ksu.9152youxi.cn

[S03] C：读入整数
来源：http://iyn.svipenyu.cn


<!-- 参考信息 -->