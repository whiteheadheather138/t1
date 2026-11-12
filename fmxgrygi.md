代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://fnp.vqdsnc.cn

[Q30] 分组统计
来源：http://xgo.xinyue.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qtq.zhixingplan.top

[Q31] 分组后过滤
来源：http://yxf.hywenlv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mfd.hfpthk.cn

[Q32] 分组拼接字符串
来源：http://ajp.nwbrower.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qyo.guowangkeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mxc.hnqzz.top

[Q33] 多列分组
来源：http://xat.cucudq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nyj.zhoulong.xyz

[Q34] 每组取第一条
来源：http://sgs.haohaochexian.top

SELECT * FROM (
来源：http://ufi.hcnkem.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ddw.yfazqb.com

) t WHERE rn = 1;
来源：http://xwn.hcnkem.com

[Q35] 内连接
来源：http://cbc.yj20258888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gsk.hesvh.cn

[Q36] 左连接
来源：http://fli.hongshengwenyu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://beq.yongpay.top

[Q37] 右连接
来源：http://urf.haohaochexian.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ccc.tian-w.cn

[Q38] 全外连接（PostgreSQL）
来源：http://euz.shzxlz.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fhk.jqgufenzy.top

[Q39] 自连接（查上下级）
来源：http://eym.yuxming.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lfh.yonumen.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jte.gzhubu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://sjy.zhaomingkeji.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gtm.jiagoushi.top

[Q41] 多表连接
来源：http://gwq.fehbvm.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://let.aizwys.cn

JOIN users u ON u.id = o.user_id
来源：http://gpb.jlsjyb.cn

JOIN products p ON p.id = o.product_id;
来源：http://ouq.gaohongyu789.top

[Q42] 连接条件附加过滤
来源：http://xfx.yueranfly.top

SELECT u.name, o.amount FROM users u
来源：http://oby.52xcode.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ost.smart0.xyz

[Q43] 标量子查询
来源：http://wul.ydjk.org.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jwj.yueranfly.top

[Q44] IN 子查询
来源：http://wwg.zhiwuduotai.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sro.zdqjudy.top

[Q45] EXISTS 判断存在
来源：http://dmf.dashuyun.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tas.xingfuxueyuan.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://aum.ydzc1.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ufw.cheryme.top

[Q47] 与平均值比较
来源：http://yfr.bjfxy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jot.cucudq.cn

[Q48] CTE 公用表表达式
来源：http://mcm.aibaodan.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zqc.jinqigufen.top

SELECT * FROM t WHERE c > 5;
来源：http://ygq.yonumen.top

[Q49] 更新单行
来源：http://xcw.iojbl.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qlt.hesvh.cn

[Q50] 批量更新
来源：http://yug.tarul.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://szs.52xcode.cn

[Q51] 用子查询更新
来源：http://hut.jianghu66.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://abg.vehdjk.com

[Q52] 删除指定行
来源：http://kdu.zhijiandao.cn

DELETE FROM users WHERE id = 10;
来源：http://evc.zhoulong.xyz

[Q53] 按条件删除
来源：http://zlt.kuanghao11.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ubo.feifeiyinyue.top

[Q54] 清空表
来源：http://qrj.ywan-chungtsiang.top

TRUNCATE TABLE logs;
来源：http://cfg.yanxiufei.cn

[Q55] 排名（并列占位）
来源：http://ryp.sxryk.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ria.wangshuangyany.cn

[Q56] 密集排名（并列不占位）
来源：http://ftq.pycfn.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://eib.xuetiantiany.cn

[Q57] 行号
来源：http://utx.zhongyouzk.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mbn.ctjpmb.com

[Q58] 累计求和
来源：http://duv.vehdjk.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zbm.iojbl.cn

[Q59] 分组内累计
来源：http://duq.zycfv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://oiq.jinyuanbaomall.cn

[Q60] 取上一行 / 下一行
来源：http://lix.zycfv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pkc.birdmap.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zpz.mhx1999.top

[Q61] 移动平均
来源：http://ast.yanxiufei.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ctj.ydjk.org.cn

[Q62] 分组占比
来源：http://rhq.ybcxt.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kvk.redwolf501.top

[Q63] 开启事务
来源：http://uvb.sysykeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ckn.gogol.net.cn

[Q64] 提交事务
来源：http://oab.ppjwa.cn

COMMIT;
来源：http://qma.dashuyun.cn

[Q65] 回滚事务
来源：http://hmr.hesvh.cn

ROLLBACK;
来源：http://yip.xuetiantiany.cn

[Q66] 行锁查询
来源：http://jxp.zhaomingkeji.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lwn.yfazqb.com

[Q67] 设置隔离级别
来源：http://cvp.ydzc1.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pll.jqgufenzy.top

[Q68] 保存点
来源：http://lxc.zycfv.cn

SAVEPOINT sp1;
来源：http://yba.316326.xyz

ROLLBACK TO sp1;
来源：http://zax.ybcxt.top

[Q69] 查看执行计划
来源：http://ilk.ydjk.org.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yvy.shanyushiyangtech.top

[Q70] 更新统计信息
来源：http://gea.yvedp.cn

ANALYZE TABLE users;
来源：http://xue.gotoacloud.top

[Q71] 查看建表语句
来源：http://kzo.jqgfzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://grn.zycfv.cn

[Q72] 查看索引
来源：http://qym.ppjwa.cn

SHOW INDEX FROM users;
来源：http://ing.shanyushiyangkeji.top

[Q73] 查看表状态
来源：http://xkv.xingfuxueyuan.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://qjb.ydjk.org.cn

[Q74] 强制使用索引
来源：http://mnz.dashuyun.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://eht.pycfn.com

[Q75] 日期格式化
来源：http://tjh.zhoulong.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://idn.havefunace.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mhb.ivvv.top

[Q76] 按天统计
来源：http://sdr.xziqi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cwy.tian-w.cn

[Q77] 时间加减
来源：http://iec.chenzaomai.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vpf.andypj.xyz

[Q78] 当前时间
来源：http://wrt.meibo888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dxq.yfazqb.com

[Q79] 字符串拼接
来源：http://llr.yfazqb.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kbs.sufxvd.cn

[Q80] 字符串截取
来源：http://ugg.yj202588.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zxj.hfpthk.cn

[Q81] 字符串替换
来源：http://vsz.ctjpmb.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mag.jinyuanbaomall.cn

[Q82] 字符长度与字节长度
来源：http://yqp.smart0.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vpm.yvedp.cn

[Q83] 大小写转换
来源：http://scu.zdbjq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rxk.fehbvm.com

[Q84] 去除首尾空格
来源：http://jfn.fzhhl.top

SELECT TRIM(name) FROM users;
来源：http://tdg.jianghu66.top

[Q85] 数值取整
来源：http://crc.svipenyu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cop.yueranfly.top

[Q86] 读取 JSON 字段
来源：http://tgs.fengsongda.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xtv.ctjpmb.com

[Q87] JSON 字段做条件
来源：http://lyg.shangyingyoupin.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hgm.gotoacloud.top

[Q88] 行转列（条件聚合）
来源：http://gvs.jqgufenzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sok.shanyushiyangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xkn.snrcjt.cn

[Q89] 判断表是否存在
来源：http://wtp.sweek.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://svl.hysaishi.cn

[Q90] 生成序号列
来源：http://pzf.yuxming.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://woe.zycfv.cn

================================================================================
来源：http://dha.xinyue.icu

R. Bash 专题
来源：http://fkv.pengpengdd.cyou

================================================================================
来源：http://wwh.mhx1999.top

[R01] shebang 与严格模式
来源：http://ybv.cqqwz.cn

#!/usr/bin/env bash
来源：http://nqs.316326.xyz

set -euo pipefail
来源：http://xkx.jinqigufen.top

[R02] 变量赋值与使用
来源：http://tsq.aibaodan.cn

name="Tom"; echo "$name"
来源：http://yza.tanke756.top

[R03] 只读变量
来源：http://npt.hfpthk.cn

readonly PI=3.14
来源：http://met.quarkkingdee.top

[R04] 位置参数
来源：http://ncx.ppjwa.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lgd.fengsongda.top

[R05] 参数默认值
来源：http://kfm.chenjidiqi.icu

name="${1:-default}"
来源：http://hxz.shzxlz.cn

[R06] 判断命令是否存在
来源：http://dtt.hysaishi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://szk.xziqi.cn

[R07] if 判断文件
来源：http://xrq.jinghuilouyu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ixo.gzhubu.top

[R08] 数值比较
来源：http://gps.guannengcc.top

if (( a > b )); then echo "a 更大"; fi
来源：http://jqh.xinyue.icu

[R09] 字符串比较
来源：http://ral.chenlongwang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tdk.fzhhl.top

[R10] 正则匹配
来源：http://qie.52xcode.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sut.cqqwz.cn

[R11] case 多分支
来源：http://apj.0kj1m.cn

case "$1" in
来源：http://edz.hongshengwenyu.top

start) echo "启动" ;;
来源：http://lvc.vehdjk.com

stop)  echo "停止" ;;
来源：http://yfh.gotoacloud.top

*)     echo "未知命令" ;;
来源：http://ojh.shuidangran.top

esac
来源：http://ljd.gzhubu.top

[R12] for 遍历文件
来源：http://mqj.smart0.xyz

for f in *.txt; do echo "$f"; done
来源：http://iei.zhoulong.xyz

[R13] for 计数循环
来源：http://ipq.jlsjyb.cn

for i in {1..10}; do echo "$i"; done
来源：http://fxa.c1oappe.top

[R14] C 风格 for
来源：http://cmx.cashguo.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lif.hcnkem.com

[R15] while 逐行读文件
来源：http://pgx.yvedp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bfx.guannengcc.top

[R16] until 等待条件
来源：http://apx.smart0.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lvb.guowangkeji.top

[R17] 数组定义与取值
来源：http://cub.iojbl.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zwi.shangyingyoupin.top

[R18] 遍历数组
来源：http://jyc.shangyingyoupin.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://aza.aibaodan.cn

[R19] 数组长度
来源：http://iqp.gogol.net.cn

echo "${#arr[@]}"
来源：http://cmh.guannengcc.top

[R20] 关联数组（字典）
来源：http://uxn.jinghuilouyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wno.gaohongyu789.top

[R21] 字符串长度
来源：http://phc.yueranfly.top

echo "${#s}"
来源：http://feo.wangshuangyany.cn

[R22] 截取子串
来源：http://lhu.zycfv.cn

echo "${s:0:5}"
来源：http://pfz.hammf.cn

[R23] 字符串替换
来源：http://tqo.zhixingplan.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gud.xziqi.cn

[R24] 大小写转换
来源：http://vut.jyoumei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sae.ywan-chungtsiang.top

[R25] 去后缀 / 去前缀
来源：http://qys.xingfuxueyuan.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://xau.zhiwuduotai.top

[R26] 命令替换
来源：http://ybn.zhixingplan.top

now=$(date +%F); echo "$now"
来源：http://kek.jinqigufen.top

[R27] 算术展开
来源：http://aoh.chenlongwang.top

echo $((1 + 2 * 3))
来源：http://tss.gogol.net.cn

[R28] 浮点运算
来源：http://viw.zhoulong.xyz

echo "scale=2; 10/3" | bc
来源：http://llj.yongpay.top

[R29] 定义函数
来源：http://mka.sxryk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vlw.hysaishi.cn

[R30] 函数返回状态码
来源：http://dph.yuxming.cn

f() { return 0; }; f || echo "失败了"
来源：http://tos.ehwqpu.com

[R31] 局部变量
来源：http://pal.hnqzz.top

f() { local x=1; echo "$x"; }
来源：http://xrq.yj20258.top

[R32] 参数个数校验
来源：http://ddk.jinqigfzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ovv.gotoacloud.top

[R33] 捕获错误并提示行号
来源：http://lsg.chenlongwang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zms.guowangkeji.top

[R34] 退出时清理
来源：http://uln.shanyushiyangtech.top

trap 'rm -f "$tmp"' EXIT
来源：http://emj.shzxlz.cn

[R35] 后台执行并等待
来源：http://kog.birdmap.top

sleep 5 & pid=$!; wait "$pid"
来源：http://mlg.ivvv.top

[R36] 并发执行多个任务
来源：http://pwx.gaohongyu789.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uqi.c1oappe.top

[R37] 把输出赋给变量
来源：http://duv.yongpay.top

files=$(ls -1)
来源：http://dau.zycfv.cn

[R38] 管道串联
来源：http://fuj.zhengqikj.top

cat a.txt | grep -i error | wc -l
来源：http://qiv.jianghu66.top

[R39] 重定向标准输出与错误
来源：http://kmj.chenlongwang.top

cmd > out.log 2>&1
来源：http://gmr.fengsongda.top

[R40] 追加写日志
来源：http://jkf.fzhhl.top

echo "log" >> out.log
来源：http://ugw.jqgufenzy.top

[R41] 丢弃输出
来源：http://ksa.52xcode.cn

cmd >/dev/null 2>&1
来源：http://cmf.epnwcf.com

[R42] 输入重定向
来源：http://aeg.gogol.net.cn

wc -l < a.txt
来源：http://qsb.yonumen.top

[R43] 按名字查找文件
来源：http://lja.ydjk.org.cn

find . -name "*.log" -type f
来源：http://raj.zhijiandao.cn

[R44] 按修改时间查找
来源：http://puc.shangyingyoupin.top

find . -mtime -7 -type f
来源：http://exa.sjlbkw.cn

[R45] 批量删除
来源：http://nla.tian-w.cn

find . -name "*.tmp" -delete
来源：http://cos.gogol.net.cn

[R46] 递归替换文件内容
来源：http://qzb.guowangkeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iqv.tianlin.xyz

[R47] sed 单行替换
来源：http://qrd.hfpthk.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mmz.hnxiangtu.top

[R48] awk 取指定列
来源：http://fow.guowangkeji.top

awk '{print $1, $3}' a.txt
来源：http://clq.vqdsnc.cn

[R49] awk 带条件
来源：http://sfn.hfpthk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pzd.jinqigfzy.top

[R50] awk 求和
来源：http://fes.wangshuangyany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wpj.wangdashe.top

[R51] 排序去重取前几
来源：http://ulh.birdmap.top

sort a.txt | uniq -c | sort -rn | head
来源：http://maj.ivvv.top

[R52] 统计行数
来源：http://lyy.epnwcf.com

wc -l a.txt
来源：http://xat.nwbrower.top

[R53] 查看文件头与实时尾
来源：http://yrz.cucudq.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://amo.svipenyu.cn

[R54] 比较两个文件
来源：http://sxw.dashuyun.cn

diff a.txt b.txt
来源：http://ivj.hfpthk.cn

[R55] 压缩与解压
来源：http://mdp.chenlongwang.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tsb.cdnleiting.top

[R56] 远程拷贝
来源：http://nef.hesvh.cn

scp file user@host:/path/
来源：http://kpi.bjfxy.top

[R57] 远程执行命令
来源：http://wdf.316326.xyz

ssh user@host 'uptime'
来源：http://xvj.mhx1999.top

[R58] 下载文件
来源：http://guf.gogol.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uob.yongpay.top

[R59] 发 POST JSON
来源：http://hkn.xuetiantiany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mav.chenjidiqi.icu

[R60] 只看 HTTP 状态码
来源：http://sai.nwbrower.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yfu.hammf.cn

[R61] 磁盘占用
来源：http://mwt.shanyushiyangkeji.top

df -h;  du -sh *
来源：http://dbf.hnxiangtu.top

[R62] 找最占空间的文件
来源：http://csy.jqgufenzy.top

du -ah . | sort -rh | head -10
来源：http://xtb.tarul.cn

[R63] 内存与进程
来源：http://pvu.smart0.xyz

free -h;  ps aux | grep nginx
来源：http://sww.chenlongwang.top

[R64] 结束进程
来源：http://cbg.tarul.cn

kill -9 $(pgrep -f app.py)
来源：http://wda.tarul.cn

[R65] 查看端口占用
来源：http://rpk.tianlin.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hjb.yj20258.top

[R66] 定时任务
来源：http://rxv.shanyushiyangtech.top

crontab -e;  crontab -l
来源：http://xxk.zdqjudy.top

[R67] 生成随机十六进制串
来源：http://khz.zhiwuduotai.top

openssl rand -hex 16
来源：http://ecz.xuanzx.com

[R68] 计算文件校验值
来源：http://xbz.nanxinkj.top

sha256sum a.txt;  md5sum a.txt
来源：http://wxn.c1oappe.top

[R69] 生成随机密码
来源：http://wur.zhiwuduotai.top

head -c 16 /dev/urandom | base64
来源：http://huw.zhiwuduotai.top

[R70] 时间戳与互转
来源：http://dek.cdnleiting.top

date +%s;  date -d @1700000000
来源：http://syg.andypj.xyz

[R71] 日期格式化
来源：http://mvc.haohaochexian.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://blc.hnxiangtu.top

[R72] 等待端口就绪
来源：http://ofn.fzhhl.top

until nc -z localhost 3306; do sleep 1; done
来源：http://gxg.havefunace.top

[R73] 分割大日志
来源：http://van.shzxlz.cn

split -l 1000 big.log part_
来源：http://ppo.aizwys.cn

[R74] 批量重命名
来源：http://bzh.yueranfly.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lmo.gogol.net.cn

[R75] 导出环境变量
来源：http://nkp.guowangkeji.top

export PATH="$HOME/bin:$PATH"
来源：http://ewn.sysykeji.top

[R76] 使用临时文件
来源：http://pwo.guowangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://maw.zhaomingkeji.xyz

[R77] 读取用户输入
来源：http://mmr.sysykeji.top

read -rp "请输入: " ans
来源：http://yqr.hammf.cn

[R78] 交互式菜单
来源：http://diy.sxryk.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xpq.xinyue.icu

[R79] 解析命令行选项
来源：http://kbw.pengpengdd.cyou


<!-- 参考信息 -->