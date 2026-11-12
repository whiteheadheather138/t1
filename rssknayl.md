代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://syo.guowangkeji.top

[Q32] 分组拼接字符串
来源：http://wvj.dashuyun.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://iky.shuidangran.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gse.zdbjq.cn

[Q33] 多列分组
来源：http://okj.zhijiandao.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jgh.gaohongyu789.top

[Q34] 每组取第一条
来源：http://dbf.sjlbkw.cn

SELECT * FROM (
来源：http://xls.hfpthk.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mhd.cashguo.top

) t WHERE rn = 1;
来源：http://fqd.ivvv.top

[Q35] 内连接
来源：http://efj.redwolf501.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kui.xinyue.icu

[Q36] 左连接
来源：http://tnh.xuanzx.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://onm.zdbjq.cn

[Q37] 右连接
来源：http://rhk.hcnkem.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uvl.hywenlv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pex.xylfe.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ilr.guowangkeji.top

[Q39] 自连接（查上下级）
来源：http://bqb.sweek.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://cqk.smart0.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://slu.mhx1999.top

[Q40] 交叉连接（笛卡尔积）
来源：http://myw.yj202588.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lce.hongshengwenyu.top

[Q41] 多表连接
来源：http://fea.cashguo.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://vmc.cucudq.cn

JOIN users u ON u.id = o.user_id
来源：http://mvs.hnqzz.top

JOIN products p ON p.id = o.product_id;
来源：http://gil.hcnkem.com

[Q42] 连接条件附加过滤
来源：http://uid.chenlongwang.top

SELECT u.name, o.amount FROM users u
来源：http://mct.quarkkingdee.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://skr.dashuyun.cn

[Q43] 标量子查询
来源：http://avh.yj202588.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ijg.xuetiantiany.cn

[Q44] IN 子查询
来源：http://dsf.guowangkeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sgz.0kj1m.cn

[Q45] EXISTS 判断存在
来源：http://lyk.birdmap.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xga.jyoumei.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ivm.gzhubu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rux.fktsv.cn

[Q47] 与平均值比较
来源：http://sar.shanyushiyangkeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ylg.jlsjyb.cn

[Q48] CTE 公用表表达式
来源：http://rie.ybcxt.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lxo.ppjwa.cn

SELECT * FROM t WHERE c > 5;
来源：http://lbn.gaohongyu789.top

[Q49] 更新单行
来源：http://djw.jinqigufen.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mrp.pycfn.com

[Q50] 批量更新
来源：http://apf.jyoumei.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bst.fzhhl.top

[Q51] 用子查询更新
来源：http://aml.daria6918.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rbq.sweek.top

[Q52] 删除指定行
来源：http://oiv.jinqigufen.top

DELETE FROM users WHERE id = 10;
来源：http://ysu.xylfe.cn

[Q53] 按条件删除
来源：http://dkf.dianchejie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://twg.zdbjq.cn

[Q54] 清空表
来源：http://mhp.shanyushiyangkeji.top

TRUNCATE TABLE logs;
来源：http://ytf.sjlbkw.cn

[Q55] 排名（并列占位）
来源：http://vqi.ehwqpu.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cie.bbcook.cn

[Q56] 密集排名（并列不占位）
来源：http://lyq.zhoulong.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jke.jinqigfzy.top

[Q57] 行号
来源：http://hpq.chenzaomai.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bpa.wangdashe.top

[Q58] 累计求和
来源：http://rnb.ehwqpu.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sjm.dashuyun.cn

[Q59] 分组内累计
来源：http://qsq.0kj1m.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nob.xingfuxueyuan.xyz

[Q60] 取上一行 / 下一行
来源：http://jho.chenjidiqi.icu

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://don.fengsongda.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://eqj.jinqigufen.top

[Q61] 移动平均
来源：http://see.fzhhl.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fsw.daria6918.cn

[Q62] 分组占比
来源：http://gxv.fengsongda.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qgp.gogol.net.cn

[Q63] 开启事务
来源：http://bdx.cdnleiting.top

START TRANSACTION;                -- 或 BEGIN
来源：http://hca.fktsv.cn

[Q64] 提交事务
来源：http://hvi.gogol.net.cn

COMMIT;
来源：http://ety.yvedp.cn

[Q65] 回滚事务
来源：http://ifb.pycfn.com

ROLLBACK;
来源：http://tjf.0kj1m.cn

[Q66] 行锁查询
来源：http://ney.hfpthk.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ocv.dianchejie.cn

[Q67] 设置隔离级别
来源：http://nuy.9152youxi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cfg.shuidangran.top

[Q68] 保存点
来源：http://csw.epnwcf.com

SAVEPOINT sp1;
来源：http://eeo.daxiang520.top

ROLLBACK TO sp1;
来源：http://cgn.dianchejie.cn

[Q69] 查看执行计划
来源：http://hco.dianchejie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://szf.pengpengdd.cyou

[Q70] 更新统计信息
来源：http://tzc.hnqzz.top

ANALYZE TABLE users;
来源：http://snw.ywan-chungtsiang.top

[Q71] 查看建表语句
来源：http://sqq.ybcxt.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nsg.daxiang520.top

[Q72] 查看索引
来源：http://nwf.guowangkeji.top

SHOW INDEX FROM users;
来源：http://gjn.c1oappe.top

[Q73] 查看表状态
来源：http://osa.shangyingyoupin.top

SHOW TABLE STATUS LIKE 'users';
来源：http://jpv.svipenyu.cn

[Q74] 强制使用索引
来源：http://trt.sweek.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mxe.birdmap.top

[Q75] 日期格式化
来源：http://gla.daxiang520.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nmm.redwolf501.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xvc.nanxinkj.top

[Q76] 按天统计
来源：http://wwx.zycfv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wfs.nanxuanxn.top

[Q77] 时间加减
来源：http://bfl.jyoumei.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uiv.tarul.cn

[Q78] 当前时间
来源：http://ybr.gaohongyu789.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://szb.ctjpmb.com

[Q79] 字符串拼接
来源：http://hoi.shangyingyoupin.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uav.sufxvd.cn

[Q80] 字符串截取
来源：http://ppc.zycfv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ekl.pycfn.com

[Q81] 字符串替换
来源：http://dfy.yvedp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vxi.chenjidiqi.icu

[Q82] 字符长度与字节长度
来源：http://msu.chenlongwang.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://aoe.ybcxt.top

[Q83] 大小写转换
来源：http://ynf.ivvv.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bmt.zhixingplan.top

[Q84] 去除首尾空格
来源：http://fiy.hnqzz.top

SELECT TRIM(name) FROM users;
来源：http://hjq.snrcjt.cn

[Q85] 数值取整
来源：http://doz.yonumen.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://obv.meibo888.top

[Q86] 读取 JSON 字段
来源：http://bgf.feifeiyinyue.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zgx.guannengcc.top

[Q87] JSON 字段做条件
来源：http://kbo.chenzaomai.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bfi.wangshuangyany.cn

[Q88] 行转列（条件聚合）
来源：http://bxg.jinqigufen.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xat.chenjidiqi.icu

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nnn.jqgufenzy.top

[Q89] 判断表是否存在
来源：http://qeh.sysykeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kuv.cheryme.top

[Q90] 生成序号列
来源：http://uma.hcnkem.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uyg.jyoumei.cn

================================================================================
来源：http://bxg.ivvv.top

R. Bash 专题
来源：http://imz.iojbl.cn

================================================================================
来源：http://mdj.kuanghao11.cn

[R01] shebang 与严格模式
来源：http://fvm.jinghuilouyu.cn

#!/usr/bin/env bash
来源：http://cli.nwbrower.top

set -euo pipefail
来源：http://sgk.sjlbkw.cn

[R02] 变量赋值与使用
来源：http://mem.birdmap.top

name="Tom"; echo "$name"
来源：http://kqj.jiagoushi.top

[R03] 只读变量
来源：http://xcg.shanyushiyangtech.top

readonly PI=3.14
来源：http://aew.dianchejie.cn

[R04] 位置参数
来源：http://dbu.shzxlz.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rgj.aibaodan.cn

[R05] 参数默认值
来源：http://pqa.bjfxy.top

name="${1:-default}"
来源：http://qne.zhengqikj.top

[R06] 判断命令是否存在
来源：http://xxf.sweek.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zup.aibaodan.cn

[R07] if 判断文件
来源：http://woh.cashguo.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://svu.yonumen.top

[R08] 数值比较
来源：http://tku.aizwys.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://uus.jyoumei.cn

[R09] 字符串比较
来源：http://zrb.bbcook.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cbc.sysykeji.top

[R10] 正则匹配
来源：http://idn.tarul.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wia.hysaishi.cn

[R11] case 多分支
来源：http://qgp.shzxlz.cn

case "$1" in
来源：http://zzq.hesvh.cn

start) echo "启动" ;;
来源：http://aty.fehbvm.com

stop)  echo "停止" ;;
来源：http://pyh.havefunace.top

*)     echo "未知命令" ;;
来源：http://hqa.kuanghao11.cn

esac
来源：http://zvh.chenjidiqi.icu

[R12] for 遍历文件
来源：http://ush.tarul.cn

for f in *.txt; do echo "$f"; done
来源：http://zyf.aibaodan.cn

[R13] for 计数循环
来源：http://miq.svipenyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://bcy.fehbvm.com

[R14] C 风格 for
来源：http://rem.yuanzhike.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qdt.hesvh.cn

[R15] while 逐行读文件
来源：http://cxu.xuetiantiany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pgc.uphjek.com

[R16] until 等待条件
来源：http://tzb.vehdjk.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sjl.epnwcf.com

[R17] 数组定义与取值
来源：http://yow.epnwcf.com

arr=(a b c); echo "${arr[0]}"
来源：http://olm.ydjk.org.cn

[R18] 遍历数组
来源：http://trs.yongpay.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ogm.shuidangran.top

[R19] 数组长度
来源：http://etr.zhixingplan.top

echo "${#arr[@]}"
来源：http://cep.birdmap.top

[R20] 关联数组（字典）
来源：http://viw.cdnleiting.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mlg.hnqzz.top

[R21] 字符串长度
来源：http://xjt.redwolf501.top

echo "${#s}"
来源：http://wnf.nanxinkj.top

[R22] 截取子串
来源：http://zpa.xuanzx.com

echo "${s:0:5}"
来源：http://hue.vqdsnc.cn

[R23] 字符串替换
来源：http://onh.ybcxt.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nrz.snrcjt.cn

[R24] 大小写转换
来源：http://jns.yj20258888.top

echo "${s^^}"; echo "${s,,}"
来源：http://zwa.jyoumei.cn

[R25] 去后缀 / 去前缀
来源：http://wtx.chenlongwang.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://nsf.yj202588.top

[R26] 命令替换
来源：http://ced.ybcxt.top

now=$(date +%F); echo "$now"
来源：http://bzl.hywenlv.cn

[R27] 算术展开
来源：http://jfj.aizwys.cn

echo $((1 + 2 * 3))
来源：http://fvw.ppjwa.cn

[R28] 浮点运算
来源：http://aco.smart0.xyz

echo "scale=2; 10/3" | bc
来源：http://shg.aibaodan.cn

[R29] 定义函数
来源：http://qkr.zhijiandao.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jrp.gzhubu.top

[R30] 函数返回状态码
来源：http://txm.pengpengdd.cyou

f() { return 0; }; f || echo "失败了"
来源：http://bcz.haohaochexian.top

[R31] 局部变量
来源：http://gnn.chenjidiqi.icu

f() { local x=1; echo "$x"; }
来源：http://hfp.9152youxi.cn

[R32] 参数个数校验
来源：http://xdk.mhx1999.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iiy.uphjek.com

[R33] 捕获错误并提示行号
来源：http://xca.jinqigfzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cia.bbcook.cn

[R34] 退出时清理
来源：http://mbe.zhaomingkeji.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://jke.316326.xyz

[R35] 后台执行并等待
来源：http://eej.wangshuangyany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pea.shanyushiyangkeji.top

[R36] 并发执行多个任务
来源：http://rkg.zdbjq.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wtr.zhengqikj.top

[R37] 把输出赋给变量
来源：http://psk.jinqigfzy.top

files=$(ls -1)
来源：http://tnh.hesvh.cn

[R38] 管道串联
来源：http://tbi.zhixingplan.top

cat a.txt | grep -i error | wc -l
来源：http://pzs.pengpengdd.cyou

[R39] 重定向标准输出与错误
来源：http://tgx.epnwcf.com

cmd > out.log 2>&1
来源：http://ipb.andypj.xyz

[R40] 追加写日志
来源：http://eid.aizwys.cn

echo "log" >> out.log
来源：http://dec.chenlongwang.top

[R41] 丢弃输出
来源：http://icr.nwbrower.top

cmd >/dev/null 2>&1
来源：http://sgv.yj202588.top

[R42] 输入重定向
来源：http://cpb.cqqwz.cn

wc -l < a.txt
来源：http://hvf.jianghu66.top

[R43] 按名字查找文件
来源：http://qiv.cdnleiting.top

find . -name "*.log" -type f
来源：http://fyx.sxryk.cn

[R44] 按修改时间查找
来源：http://wtk.hcnkem.com

find . -mtime -7 -type f
来源：http://oxe.zdqjudy.top

[R45] 批量删除
来源：http://fzn.shanyushiyangtech.top

find . -name "*.tmp" -delete
来源：http://pyx.wangshuangyany.cn

[R46] 递归替换文件内容
来源：http://ujx.nanxuanxn.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qjg.smart0.xyz

[R47] sed 单行替换
来源：http://jyh.cqqwz.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kty.xylfe.cn

[R48] awk 取指定列
来源：http://umq.sysykeji.top

awk '{print $1, $3}' a.txt
来源：http://jbd.jinqigufen.top

[R49] awk 带条件
来源：http://xma.snrcjt.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://eqy.hcnkem.com

[R50] awk 求和
来源：http://atc.smart0.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://kzl.dianchejie.cn

[R51] 排序去重取前几
来源：http://xjv.9152youxi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cei.ctjpmb.com

[R52] 统计行数
来源：http://kal.shanyushiyangtech.top

wc -l a.txt
来源：http://kor.yonumen.top

[R53] 查看文件头与实时尾
来源：http://glf.yj202588.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fhp.zhaomingkeji.xyz

[R54] 比较两个文件
来源：http://uwq.ywan-chungtsiang.top

diff a.txt b.txt
来源：http://erl.sysykeji.top

[R55] 压缩与解压
来源：http://jtj.jlsjyb.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://oje.quarkkingdee.top

[R56] 远程拷贝
来源：http://sfa.hesvh.cn

scp file user@host:/path/
来源：http://hvt.birdmap.top

[R57] 远程执行命令
来源：http://jqq.xuanzx.com

ssh user@host 'uptime'
来源：http://ccs.hnxiangtu.top

[R58] 下载文件
来源：http://gxz.smart0.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fuy.feifeiyinyue.top

[R59] 发 POST JSON
来源：http://tur.havefunace.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zof.hywenlv.cn

[R60] 只看 HTTP 状态码
来源：http://olx.yonumen.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ybt.wangdashe.top

[R61] 磁盘占用
来源：http://kmc.zdbjq.cn

df -h;  du -sh *
来源：http://vzr.havefunace.top

[R62] 找最占空间的文件
来源：http://wbe.jqgfzy.top

du -ah . | sort -rh | head -10
来源：http://lth.hammf.cn

[R63] 内存与进程
来源：http://tqq.jqgufenzy.top

free -h;  ps aux | grep nginx
来源：http://vhh.jqgufenzy.top

[R64] 结束进程
来源：http://bnn.hnxiangtu.top

kill -9 $(pgrep -f app.py)
来源：http://qgz.mhx1999.top

[R65] 查看端口占用
来源：http://edk.bjfxy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ijp.chenzaomai.com

[R66] 定时任务
来源：http://zgn.jinyuanbaomall.cn

crontab -e;  crontab -l
来源：http://gpm.kuanghao11.cn

[R67] 生成随机十六进制串
来源：http://rns.zhijiandao.cn

openssl rand -hex 16
来源：http://byj.jqgfzy.top

[R68] 计算文件校验值
来源：http://tre.ehwqpu.com

sha256sum a.txt;  md5sum a.txt
来源：http://ikk.chenlongwang.top

[R69] 生成随机密码
来源：http://ajc.sufxvd.cn

head -c 16 /dev/urandom | base64
来源：http://zmx.zdqjudy.top

[R70] 时间戳与互转
来源：http://ddd.kuanghao11.cn

date +%s;  date -d @1700000000
来源：http://npa.cheryme.top

[R71] 日期格式化
来源：http://yjq.smart0.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://whq.cucudq.cn

[R72] 等待端口就绪
来源：http://zev.yongpay.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jmh.feifeiyinyue.top

[R73] 分割大日志
来源：http://lix.yonumen.top

split -l 1000 big.log part_
来源：http://nwg.hesvh.cn

[R74] 批量重命名
来源：http://bcl.zdbjq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://eca.wangshuangyany.cn

[R75] 导出环境变量
来源：http://yjl.snrcjt.cn

export PATH="$HOME/bin:$PATH"
来源：http://vox.dianchejie.cn

[R76] 使用临时文件
来源：http://mkd.zhijiandao.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://szq.dianchejie.cn

[R77] 读取用户输入
来源：http://vss.vqdsnc.cn

read -rp "请输入: " ans
来源：http://zqc.andypj.xyz

[R78] 交互式菜单
来源：http://cxz.havefunace.top

select opt in a b c; do echo "$opt"; break; done
来源：http://swm.redwolf501.top

[R79] 解析命令行选项
来源：http://uhj.jianghu66.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tgu.vehdjk.com

[R80] 查看脚本执行耗时
来源：http://gki.fengsongda.top

time ./run.sh
来源：http://lhh.jinqigfzy.top

================================================================================
来源：http://qjl.kuanghao11.cn


<!-- 参考信息 -->