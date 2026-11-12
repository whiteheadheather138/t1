代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://mvv.mhx1999.top

[Q22] 排序
来源：http://yvz.shanyushiyangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rdw.gaohongyu789.top

[Q23] 分页
来源：http://rnx.ppjwa.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kcy.cheryme.top

[Q24] 去重
来源：http://ayl.jqgfzy.top

SELECT DISTINCT city FROM users;
来源：http://paf.fengsongda.top

[Q25] 只取前 N 条
来源：http://yvs.shangyingyoupin.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vlq.fehbvm.com

[Q26] 计数
来源：http://xvv.fehbvm.com

SELECT COUNT(*) FROM users;
来源：http://rgk.ctjpmb.com

[Q27] 条件计数
来源：http://nhf.fehbvm.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ght.fehbvm.com

[Q28] 求和与平均
来源：http://pgz.52xcode.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ooo.shangyingyoupin.top

[Q29] 最大最小值
来源：http://aps.shangyingyoupin.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://iis.pengpengdd.cyou

[Q30] 分组统计
来源：http://dlc.shanyushiyangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://moz.ywan-chungtsiang.top

[Q31] 分组后过滤
来源：http://zuh.hfpthk.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yds.shuidangran.top

[Q32] 分组拼接字符串
来源：http://opw.mhx1999.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blg.hysaishi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gno.wangdashe.top

[Q33] 多列分组
来源：http://pmu.yongpay.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ivk.yj202588.top

[Q34] 每组取第一条
来源：http://tzz.vehdjk.com

SELECT * FROM (
来源：http://ypx.vehdjk.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ovq.yfazqb.com

) t WHERE rn = 1;
来源：http://qxv.hnqzz.top

[Q35] 内连接
来源：http://pcl.gzhubu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ujy.tianlin.xyz

[Q36] 左连接
来源：http://drq.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vrh.hcnkem.com

[Q37] 右连接
来源：http://asl.epnwcf.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vvr.yj20258.top

[Q38] 全外连接（PostgreSQL）
来源：http://fea.uphjek.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hsg.xingfuxueyuan.xyz

[Q39] 自连接（查上下级）
来源：http://snh.fktsv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bjq.chenzaomai.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://uur.vqdsnc.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://naw.nanxinkj.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gyp.feifeiyinyue.top

[Q41] 多表连接
来源：http://zab.shuidangran.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://fde.ivvv.top

JOIN users u ON u.id = o.user_id
来源：http://gyd.aizwys.cn

JOIN products p ON p.id = o.product_id;
来源：http://qzb.hongshengwenyu.top

[Q42] 连接条件附加过滤
来源：http://xqr.jqgfzy.top

SELECT u.name, o.amount FROM users u
来源：http://snq.316326.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kut.chenjidiqi.icu

[Q43] 标量子查询
来源：http://goi.yongpay.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jon.zycfv.cn

[Q44] IN 子查询
来源：http://xjv.yonumen.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tdi.tanke756.top

[Q45] EXISTS 判断存在
来源：http://reb.wangshuangyany.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bnw.xuanzx.com

[Q46] NOT EXISTS 判断不存在
来源：http://iku.52xcode.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ejt.yonumen.top

[Q47] 与平均值比较
来源：http://xpe.wangdashe.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vte.yongpay.top

[Q48] CTE 公用表表达式
来源：http://crv.xinyue.icu

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bxn.haohaochexian.top

SELECT * FROM t WHERE c > 5;
来源：http://psg.shanyushiyangkeji.top

[Q49] 更新单行
来源：http://zis.hesvh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rui.dashuyun.cn

[Q50] 批量更新
来源：http://rwu.52xcode.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hoq.tianlin.xyz

[Q51] 用子查询更新
来源：http://hfc.tianlin.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mcu.ydzc1.top

[Q52] 删除指定行
来源：http://kek.jinghuilouyu.cn

DELETE FROM users WHERE id = 10;
来源：http://tdd.yonumen.top

[Q53] 按条件删除
来源：http://kqu.hfpthk.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gba.bjfxy.top

[Q54] 清空表
来源：http://nak.hnxiangtu.top

TRUNCATE TABLE logs;
来源：http://dzl.yuxming.cn

[Q55] 排名（并列占位）
来源：http://ctd.sweek.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://llo.nanxuanxn.top

[Q56] 密集排名（并列不占位）
来源：http://nwb.yuxming.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://glc.snrcjt.cn

[Q57] 行号
来源：http://mdj.jinqigfzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gbh.nanxuanxn.top

[Q58] 累计求和
来源：http://lcw.quarkkingdee.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fio.hcnkem.com

[Q59] 分组内累计
来源：http://rmv.xingfuxueyuan.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ysb.xingfuxueyuan.xyz

[Q60] 取上一行 / 下一行
来源：http://rsz.hywenlv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tbs.xylfe.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://izf.ydjk.org.cn

[Q61] 移动平均
来源：http://tmt.jinghuilouyu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mpm.tarul.cn

[Q62] 分组占比
来源：http://jab.yj20258.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://itz.snrcjt.cn

[Q63] 开启事务
来源：http://exr.zdbjq.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lgy.sweek.top

[Q64] 提交事务
来源：http://yvb.nwbrower.top

COMMIT;
来源：http://qnn.chenjidiqi.icu

[Q65] 回滚事务
来源：http://oir.jiagoushi.top

ROLLBACK;
来源：http://yur.xuanzx.com

[Q66] 行锁查询
来源：http://iab.yuxming.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tlm.nanxinkj.top

[Q67] 设置隔离级别
来源：http://inp.sweek.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sew.hysaishi.cn

[Q68] 保存点
来源：http://akm.zhoulong.xyz

SAVEPOINT sp1;
来源：http://hqr.zhixingplan.top

ROLLBACK TO sp1;
来源：http://con.tianlin.xyz

[Q69] 查看执行计划
来源：http://uvk.gotoacloud.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ese.52xcode.cn

[Q70] 更新统计信息
来源：http://vtd.uphjek.com

ANALYZE TABLE users;
来源：http://vup.jinqigfzy.top

[Q71] 查看建表语句
来源：http://xjd.pycfn.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://afj.havefunace.top

[Q72] 查看索引
来源：http://dfm.jinyuanbaomall.cn

SHOW INDEX FROM users;
来源：http://qjq.316326.xyz

[Q73] 查看表状态
来源：http://wer.birdmap.top

SHOW TABLE STATUS LIKE 'users';
来源：http://zge.yueranfly.top

[Q74] 强制使用索引
来源：http://xlz.pengpengdd.cyou

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uqe.snrcjt.cn

[Q75] 日期格式化
来源：http://alp.guannengcc.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ftl.ydjk.org.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://utw.yfazqb.com

[Q76] 按天统计
来源：http://lwx.yanxiufei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pqa.yvedp.cn

[Q77] 时间加减
来源：http://kbx.yanxiufei.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ubn.yj202588.top

[Q78] 当前时间
来源：http://huh.chenzaomai.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pyr.xuanzx.com

[Q79] 字符串拼接
来源：http://zma.nwbrower.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ray.jianghu66.top

[Q80] 字符串截取
来源：http://ybe.sxryk.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ehr.xingfuxueyuan.xyz

[Q81] 字符串替换
来源：http://cuf.xuanzx.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pjc.jqgufenzy.top

[Q82] 字符长度与字节长度
来源：http://yfp.pengpengdd.cyou

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ggi.wangshuangyany.cn

[Q83] 大小写转换
来源：http://vvj.quarkkingdee.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://smi.hfpthk.cn

[Q84] 去除首尾空格
来源：http://jda.shanyushiyangtech.top

SELECT TRIM(name) FROM users;
来源：http://blg.redwolf501.top

[Q85] 数值取整
来源：http://sxo.zdbjq.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hpq.daria6918.cn

[Q86] 读取 JSON 字段
来源：http://flv.zhaomingkeji.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kjf.hfpthk.cn

[Q87] JSON 字段做条件
来源：http://suk.yangfankeji.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://aiy.meibo888.top

[Q88] 行转列（条件聚合）
来源：http://zim.fengsongda.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gfi.ybcxt.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://weu.yonumen.top

[Q89] 判断表是否存在
来源：http://lrr.ctjpmb.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wwz.chenzaomai.com

[Q90] 生成序号列
来源：http://miu.feifeiyinyue.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jax.hysaishi.cn

================================================================================
来源：http://ajj.sxryk.cn

R. Bash 专题
来源：http://blp.hammf.cn

================================================================================
来源：http://tcj.snrcjt.cn

[R01] shebang 与严格模式
来源：http://gwh.xuetiantiany.cn

#!/usr/bin/env bash
来源：http://yyz.0kj1m.cn

set -euo pipefail
来源：http://pix.daxiang520.top

[R02] 变量赋值与使用
来源：http://ziy.yj20258888.top

name="Tom"; echo "$name"
来源：http://qcw.tarul.cn

[R03] 只读变量
来源：http://aih.nwbrower.top

readonly PI=3.14
来源：http://gcr.dianchejie.cn

[R04] 位置参数
来源：http://ytn.gaohongyu789.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://brw.jinqigfzy.top

[R05] 参数默认值
来源：http://gur.aizwys.cn

name="${1:-default}"
来源：http://fvo.yonumen.top

[R06] 判断命令是否存在
来源：http://ozi.chenjidiqi.icu

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lqv.jqgufenzy.top

[R07] if 判断文件
来源：http://kvr.fengsongda.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uvm.ybcxt.top

[R08] 数值比较
来源：http://fbz.hfpthk.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qln.jqgufenzy.top

[R09] 字符串比较
来源：http://wkf.tian-w.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ojw.daxiang520.top

[R10] 正则匹配
来源：http://ncq.bbcook.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tis.yueranfly.top

[R11] case 多分支
来源：http://rzd.yj20258.top

case "$1" in
来源：http://nlp.ehwqpu.com

start) echo "启动" ;;
来源：http://hky.dianchejie.cn

stop)  echo "停止" ;;
来源：http://fmt.daxiang520.top

*)     echo "未知命令" ;;
来源：http://sle.smart0.xyz

esac
来源：http://toc.gzhubu.top

[R12] for 遍历文件
来源：http://inj.gotoacloud.top

for f in *.txt; do echo "$f"; done
来源：http://ifi.sjlbkw.cn

[R13] for 计数循环
来源：http://tdv.cheryme.top

for i in {1..10}; do echo "$i"; done
来源：http://csy.guowangkeji.top

[R14] C 风格 for
来源：http://igx.smart0.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://swp.yongpay.top

[R15] while 逐行读文件
来源：http://lrk.hongshengwenyu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://usr.xinyue.icu

[R16] until 等待条件
来源：http://kqf.pengpengdd.cyou

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wry.uphjek.com

[R17] 数组定义与取值
来源：http://ldz.yueranfly.top

arr=(a b c); echo "${arr[0]}"
来源：http://iom.fengsongda.top

[R18] 遍历数组
来源：http://ymc.uphjek.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xhg.jqgfzy.top

[R19] 数组长度
来源：http://xpp.zdqjudy.top

echo "${#arr[@]}"
来源：http://nrk.yj20258888.top

[R20] 关联数组（字典）
来源：http://lhh.ppjwa.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://foi.nanxinkj.top

[R21] 字符串长度
来源：http://kno.ydzc1.top

echo "${#s}"
来源：http://swm.mhx1999.top

[R22] 截取子串
来源：http://pqu.zdbjq.cn

echo "${s:0:5}"
来源：http://ubd.chenjidiqi.icu

[R23] 字符串替换
来源：http://ywo.yfazqb.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://frx.aizwys.cn

[R24] 大小写转换
来源：http://itz.jqgufenzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://iun.tanke756.top

[R25] 去后缀 / 去前缀
来源：http://fva.yj20258.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://qfl.cashguo.top

[R26] 命令替换
来源：http://ikj.xziqi.cn

now=$(date +%F); echo "$now"
来源：http://hdf.hammf.cn

[R27] 算术展开
来源：http://fml.yj20258888.top

echo $((1 + 2 * 3))
来源：http://nql.zhongyouzk.top

[R28] 浮点运算
来源：http://tqc.hammf.cn

echo "scale=2; 10/3" | bc
来源：http://lmd.havefunace.top

[R29] 定义函数
来源：http://fhk.nanxuanxn.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gaq.pengpengdd.cyou

[R30] 函数返回状态码
来源：http://gzv.daria6918.cn

f() { return 0; }; f || echo "失败了"
来源：http://lse.vqdsnc.cn

[R31] 局部变量
来源：http://tbc.guannengcc.top

f() { local x=1; echo "$x"; }
来源：http://mjp.guannengcc.top

[R32] 参数个数校验
来源：http://mrg.haohaochexian.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vxx.shangyingyoupin.top

[R33] 捕获错误并提示行号
来源：http://fgw.chenlongwang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yqj.jlsjyb.cn

[R34] 退出时清理
来源：http://rhg.dashuyun.cn

trap 'rm -f "$tmp"' EXIT
来源：http://inz.yuanzhike.top

[R35] 后台执行并等待
来源：http://uec.zhoulong.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://oea.shzxlz.cn

[R36] 并发执行多个任务
来源：http://qss.yj202588.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nbg.wangdashe.top

[R37] 把输出赋给变量
来源：http://vui.yj20258888.top

files=$(ls -1)
来源：http://vlb.haohaochexian.top

[R38] 管道串联
来源：http://dog.dashuyun.cn

cat a.txt | grep -i error | wc -l
来源：http://dcc.zhiwuduotai.top

[R39] 重定向标准输出与错误
来源：http://ewf.jqgfzy.top

cmd > out.log 2>&1
来源：http://ebh.shanyushiyangtech.top

[R40] 追加写日志
来源：http://och.redwolf501.top

echo "log" >> out.log
来源：http://ikg.shanyushiyangtech.top

[R41] 丢弃输出
来源：http://ovf.daxiang520.top

cmd >/dev/null 2>&1
来源：http://tgf.sxryk.cn

[R42] 输入重定向
来源：http://hjl.hysaishi.cn

wc -l < a.txt
来源：http://zmj.pycfn.com

[R43] 按名字查找文件
来源：http://xyy.uphjek.com

find . -name "*.log" -type f
来源：http://nfh.jiagoushi.top

[R44] 按修改时间查找
来源：http://dpj.gaohongyu789.top

find . -mtime -7 -type f
来源：http://jky.ppjwa.cn

[R45] 批量删除
来源：http://lpm.yj202588.top

find . -name "*.tmp" -delete
来源：http://uqu.tanke756.top

[R46] 递归替换文件内容
来源：http://wce.yvedp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vto.xziqi.cn

[R47] sed 单行替换
来源：http://klr.yj20258.top

sed -i 's/foo/bar/g' a.txt
来源：http://vyb.guowangkeji.top

[R48] awk 取指定列
来源：http://gye.shuidangran.top

awk '{print $1, $3}' a.txt
来源：http://gmy.yj20258888.top

[R49] awk 带条件
来源：http://rdq.xinyue.icu

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fcd.jlsjyb.cn

[R50] awk 求和
来源：http://ygk.zdqjudy.top

awk '{s += $2} END {print s}' a.txt
来源：http://zns.jinqigfzy.top

[R51] 排序去重取前几
来源：http://udm.ctjpmb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://gry.jianghu66.top

[R52] 统计行数
来源：http://lgm.sweek.top

wc -l a.txt
来源：http://ban.yonumen.top

[R53] 查看文件头与实时尾
来源：http://evn.haohaochexian.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xkh.jqgfzy.top

[R54] 比较两个文件
来源：http://ijl.xziqi.cn

diff a.txt b.txt
来源：http://sar.zhijiandao.cn

[R55] 压缩与解压
来源：http://puf.ywan-chungtsiang.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uhr.hongshengwenyu.top

[R56] 远程拷贝
来源：http://zik.iojbl.cn

scp file user@host:/path/
来源：http://vzd.cheryme.top

[R57] 远程执行命令
来源：http://luk.guannengcc.top

ssh user@host 'uptime'
来源：http://cvy.sufxvd.cn

[R58] 下载文件
来源：http://mgs.tian-w.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ktm.yongpay.top

[R59] 发 POST JSON
来源：http://xpg.svipenyu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cmw.jyoumei.cn

[R60] 只看 HTTP 状态码
来源：http://aut.ctjpmb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vlj.9152youxi.cn

[R61] 磁盘占用
来源：http://zed.chenjidiqi.icu

df -h;  du -sh *
来源：http://afg.hesvh.cn

[R62] 找最占空间的文件
来源：http://lsc.chenjidiqi.icu

du -ah . | sort -rh | head -10
来源：http://lmo.jianghu66.top

[R63] 内存与进程
来源：http://lrl.xingfuxueyuan.xyz

free -h;  ps aux | grep nginx
来源：http://uuj.aizwys.cn

[R64] 结束进程
来源：http://nxn.c1oappe.top

kill -9 $(pgrep -f app.py)
来源：http://bju.zhiwuduotai.top

[R65] 查看端口占用
来源：http://jzd.snrcjt.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kbj.birdmap.top

[R66] 定时任务
来源：http://ttg.hcnkem.com

crontab -e;  crontab -l
来源：http://kst.wangshuangyany.cn

[R67] 生成随机十六进制串
来源：http://sjp.xinyue.icu

openssl rand -hex 16
来源：http://efy.zhengqikj.top

[R68] 计算文件校验值
来源：http://jbr.aibaodan.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vny.hcnkem.com

[R69] 生成随机密码
来源：http://lze.hcnkem.com

head -c 16 /dev/urandom | base64
来源：http://diq.ivvv.top

[R70] 时间戳与互转
来源：http://ogh.jinyuanbaomall.cn

date +%s;  date -d @1700000000
来源：http://amh.fzhhl.top

[R71] 日期格式化
来源：http://efv.zdqjudy.top


<!-- 参考信息 -->