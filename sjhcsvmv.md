代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wjz.tanke756.top

[Q20] IN 列表
来源：http://tod.jiagoushi.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zul.gzhubu.top

[Q21] 空值判断
来源：http://axk.hcnkem.com

SELECT * FROM users WHERE email IS NULL;
来源：http://zyj.pengpengdd.cyou

[Q22] 排序
来源：http://hjg.xingfuxueyuan.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://iya.smart0.xyz

[Q23] 分页
来源：http://kgo.hesvh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mxn.sysykeji.top

[Q24] 去重
来源：http://knd.ivvv.top

SELECT DISTINCT city FROM users;
来源：http://bfz.ydzc1.top

[Q25] 只取前 N 条
来源：http://muy.ctjpmb.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wdz.hongshengwenyu.top

[Q26] 计数
来源：http://ale.hammf.cn

SELECT COUNT(*) FROM users;
来源：http://bcs.nwbrower.top

[Q27] 条件计数
来源：http://wad.fzhhl.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ftz.ybcxt.top

[Q28] 求和与平均
来源：http://ysl.fehbvm.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oej.ybcxt.top

[Q29] 最大最小值
来源：http://evi.xuetiantiany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ldf.ybcxt.top

[Q30] 分组统计
来源：http://ibn.fehbvm.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lkv.iojbl.cn

[Q31] 分组后过滤
来源：http://hui.yfazqb.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ead.zhongyouzk.top

[Q32] 分组拼接字符串
来源：http://mrq.c1oappe.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tun.gogol.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zpg.zhiwuduotai.top

[Q33] 多列分组
来源：http://gsu.ybcxt.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vnz.hcnkem.com

[Q34] 每组取第一条
来源：http://fuo.ydzc1.top

SELECT * FROM (
来源：http://cma.jinqigfzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://khc.jinghuilouyu.cn

) t WHERE rn = 1;
来源：http://gsf.sxryk.cn

[Q35] 内连接
来源：http://one.haohaochexian.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pqm.aibaodan.cn

[Q36] 左连接
来源：http://hvu.52xcode.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nzg.gogol.net.cn

[Q37] 右连接
来源：http://tzw.zhengqikj.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lgy.iojbl.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gfj.daria6918.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hka.ydjk.org.cn

[Q39] 自连接（查上下级）
来源：http://lyd.nanxinkj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://soa.0kj1m.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fih.wangshuangyany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ukf.fehbvm.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://smj.pycfn.com

[Q41] 多表连接
来源：http://ubz.aizwys.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tsh.zhengqikj.top

JOIN users u ON u.id = o.user_id
来源：http://bkg.yuxming.cn

JOIN products p ON p.id = o.product_id;
来源：http://ywa.shanyushiyangtech.top

[Q42] 连接条件附加过滤
来源：http://bhl.316326.xyz

SELECT u.name, o.amount FROM users u
来源：http://rui.tanke756.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gzj.xinyue.icu

[Q43] 标量子查询
来源：http://nfs.hnxiangtu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tir.tian-w.cn

[Q44] IN 子查询
来源：http://wfk.andypj.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ruu.jinqigufen.top

[Q45] EXISTS 判断存在
来源：http://pjz.pycfn.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zuk.ppjwa.cn

[Q46] NOT EXISTS 判断不存在
来源：http://uhx.yvedp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jqc.tarul.cn

[Q47] 与平均值比较
来源：http://umr.nwbrower.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hfu.yongpay.top

[Q48] CTE 公用表表达式
来源：http://csw.jyoumei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://woj.vehdjk.com

SELECT * FROM t WHERE c > 5;
来源：http://rqg.ydzc1.top

[Q49] 更新单行
来源：http://pvz.zycfv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ckk.sysykeji.top

[Q50] 批量更新
来源：http://cer.sysykeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://aea.sufxvd.cn

[Q51] 用子查询更新
来源：http://wat.iojbl.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gmx.hammf.cn

[Q52] 删除指定行
来源：http://rcm.zhengqikj.top

DELETE FROM users WHERE id = 10;
来源：http://lng.epnwcf.com

[Q53] 按条件删除
来源：http://tfw.tarul.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rfi.yj20258.top

[Q54] 清空表
来源：http://esi.hesvh.cn

TRUNCATE TABLE logs;
来源：http://kdf.xuanzx.com

[Q55] 排名（并列占位）
来源：http://sgb.ybcxt.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vfq.xuanzx.com

[Q56] 密集排名（并列不占位）
来源：http://tqi.cheryme.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kdy.cucudq.cn

[Q57] 行号
来源：http://sev.nanxinkj.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bfk.aibaodan.cn

[Q58] 累计求和
来源：http://bke.wangshuangyany.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ixc.fzhhl.top

[Q59] 分组内累计
来源：http://sad.ivvv.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nml.yanxiufei.cn

[Q60] 取上一行 / 下一行
来源：http://mhy.xziqi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://imd.ctjpmb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yzr.xuanzx.com

[Q61] 移动平均
来源：http://dsl.epnwcf.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://liv.sjlbkw.cn

[Q62] 分组占比
来源：http://ibj.hnxiangtu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yih.9152youxi.cn

[Q63] 开启事务
来源：http://jxf.shangyingyoupin.top

START TRANSACTION;                -- 或 BEGIN
来源：http://cis.wangdashe.top

[Q64] 提交事务
来源：http://izx.chenjidiqi.icu

COMMIT;
来源：http://huj.jinqigufen.top

[Q65] 回滚事务
来源：http://ovg.yueranfly.top

ROLLBACK;
来源：http://bpb.pengpengdd.cyou

[Q66] 行锁查询
来源：http://doc.zhengqikj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jci.cashguo.top

[Q67] 设置隔离级别
来源：http://gvx.pycfn.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://akh.tianlin.xyz

[Q68] 保存点
来源：http://oew.uphjek.com

SAVEPOINT sp1;
来源：http://mil.aibaodan.cn

ROLLBACK TO sp1;
来源：http://otq.ywan-chungtsiang.top

[Q69] 查看执行计划
来源：http://swb.fzhhl.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zjc.hnqzz.top

[Q70] 更新统计信息
来源：http://kjn.jqgufenzy.top

ANALYZE TABLE users;
来源：http://qfv.fengsongda.top

[Q71] 查看建表语句
来源：http://aaq.c1oappe.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oau.zhaomingkeji.xyz

[Q72] 查看索引
来源：http://prl.52xcode.cn

SHOW INDEX FROM users;
来源：http://kcm.hcnkem.com

[Q73] 查看表状态
来源：http://vfo.xingfuxueyuan.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://vpr.jianghu66.top

[Q74] 强制使用索引
来源：http://qdd.nanxuanxn.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wqk.guannengcc.top

[Q75] 日期格式化
来源：http://blf.tanke756.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bqz.xziqi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xzg.yongpay.top

[Q76] 按天统计
来源：http://ggd.yvedp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ppn.tanke756.top

[Q77] 时间加减
来源：http://ukm.cheryme.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rod.dianchejie.cn

[Q78] 当前时间
来源：http://wuo.0kj1m.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zwg.sysykeji.top

[Q79] 字符串拼接
来源：http://hyu.hysaishi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cka.dianchejie.cn

[Q80] 字符串截取
来源：http://omd.yj20258.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gov.tanke756.top

[Q81] 字符串替换
来源：http://ece.jinghuilouyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zzu.0kj1m.cn

[Q82] 字符长度与字节长度
来源：http://qjl.daria6918.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cey.hfpthk.cn

[Q83] 大小写转换
来源：http://slt.cucudq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rgy.ydjk.org.cn

[Q84] 去除首尾空格
来源：http://ovh.zhixingplan.top

SELECT TRIM(name) FROM users;
来源：http://lsa.zhijiandao.cn

[Q85] 数值取整
来源：http://jff.nanxinkj.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bmv.yj20258.top

[Q86] 读取 JSON 字段
来源：http://bnp.shzxlz.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uin.gotoacloud.top

[Q87] JSON 字段做条件
来源：http://pvq.zycfv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://scn.quarkkingdee.top

[Q88] 行转列（条件聚合）
来源：http://ozd.cqqwz.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bdu.yuanzhike.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ugx.yj202588.top

[Q89] 判断表是否存在
来源：http://auw.ctjpmb.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ojj.nwbrower.top

[Q90] 生成序号列
来源：http://xkr.c1oappe.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://eae.jinghuilouyu.cn

================================================================================
来源：http://btr.xziqi.cn

R. Bash 专题
来源：http://erz.zhoulong.xyz

================================================================================
来源：http://smg.yvedp.cn

[R01] shebang 与严格模式
来源：http://cgd.ivvv.top

#!/usr/bin/env bash
来源：http://kwz.zdqjudy.top

set -euo pipefail
来源：http://irr.redwolf501.top

[R02] 变量赋值与使用
来源：http://tox.pycfn.com

name="Tom"; echo "$name"
来源：http://tux.zhaomingkeji.xyz

[R03] 只读变量
来源：http://uob.yonumen.top

readonly PI=3.14
来源：http://coe.zycfv.cn

[R04] 位置参数
来源：http://tff.vqdsnc.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tqo.ybcxt.top

[R05] 参数默认值
来源：http://kfk.ywan-chungtsiang.top

name="${1:-default}"
来源：http://mks.yuxming.cn

[R06] 判断命令是否存在
来源：http://ctx.tian-w.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xvn.zhiwuduotai.top

[R07] if 判断文件
来源：http://gsv.hesvh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nua.hysaishi.cn

[R08] 数值比较
来源：http://pnr.sufxvd.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yjx.zhengqikj.top

[R09] 字符串比较
来源：http://kyk.yj20258888.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://noo.sjlbkw.cn

[R10] 正则匹配
来源：http://tln.zdqjudy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://swd.fehbvm.com

[R11] case 多分支
来源：http://bev.uphjek.com

case "$1" in
来源：http://jbz.birdmap.top

start) echo "启动" ;;
来源：http://bel.fzhhl.top

stop)  echo "停止" ;;
来源：http://kus.kuanghao11.cn

*)     echo "未知命令" ;;
来源：http://fnt.fzhhl.top

esac
来源：http://tpw.svipenyu.cn

[R12] for 遍历文件
来源：http://yzg.hcnkem.com

for f in *.txt; do echo "$f"; done
来源：http://ubm.yueranfly.top

[R13] for 计数循环
来源：http://lea.redwolf501.top

for i in {1..10}; do echo "$i"; done
来源：http://avs.tianlin.xyz

[R14] C 风格 for
来源：http://jqg.birdmap.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dsf.daxiang520.top

[R15] while 逐行读文件
来源：http://upe.aizwys.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yxk.zycfv.cn

[R16] until 等待条件
来源：http://rgh.cashguo.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kbl.smart0.xyz

[R17] 数组定义与取值
来源：http://bqh.zdqjudy.top

arr=(a b c); echo "${arr[0]}"
来源：http://qro.fehbvm.com

[R18] 遍历数组
来源：http://kfa.yuxming.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rdn.hcnkem.com

[R19] 数组长度
来源：http://cjn.52xcode.cn

echo "${#arr[@]}"
来源：http://uvn.kuanghao11.cn

[R20] 关联数组（字典）
来源：http://hnw.fengsongda.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zmi.ydzc1.top

[R21] 字符串长度
来源：http://nlt.c1oappe.top

echo "${#s}"
来源：http://bdz.shangyingyoupin.top

[R22] 截取子串
来源：http://mgs.shanyushiyangkeji.top

echo "${s:0:5}"
来源：http://adr.yanxiufei.cn

[R23] 字符串替换
来源：http://pvg.vqdsnc.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hpr.bbcook.cn

[R24] 大小写转换
来源：http://vez.ydzc1.top

echo "${s^^}"; echo "${s,,}"
来源：http://ohm.tanke756.top

[R25] 去后缀 / 去前缀
来源：http://tgt.meibo888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://qgz.zhixingplan.top

[R26] 命令替换
来源：http://eay.jyoumei.cn

now=$(date +%F); echo "$now"
来源：http://uqs.cashguo.top

[R27] 算术展开
来源：http://udb.zhaomingkeji.xyz

echo $((1 + 2 * 3))
来源：http://sna.wangshuangyany.cn

[R28] 浮点运算
来源：http://bog.bbcook.cn

echo "scale=2; 10/3" | bc
来源：http://tch.ydjk.org.cn

[R29] 定义函数
来源：http://qen.jqgufenzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bxo.yfazqb.com

[R30] 函数返回状态码
来源：http://sgb.jqgufenzy.top

f() { return 0; }; f || echo "失败了"
来源：http://zpv.wangdashe.top

[R31] 局部变量
来源：http://pjl.chenzaomai.com

f() { local x=1; echo "$x"; }
来源：http://hbk.fengsongda.top

[R32] 参数个数校验
来源：http://iqe.shanyushiyangkeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oed.fehbvm.com

[R33] 捕获错误并提示行号
来源：http://ytl.wangdashe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fqn.ivvv.top

[R34] 退出时清理
来源：http://mjh.yuxming.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kih.cqqwz.cn

[R35] 后台执行并等待
来源：http://wtw.wangshuangyany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dlv.jinyuanbaomall.cn

[R36] 并发执行多个任务
来源：http://ccz.fktsv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://whu.hnqzz.top

[R37] 把输出赋给变量
来源：http://zqb.yongpay.top

files=$(ls -1)
来源：http://ptk.yonumen.top

[R38] 管道串联
来源：http://nzx.kuanghao11.cn

cat a.txt | grep -i error | wc -l
来源：http://qsc.guannengcc.top

[R39] 重定向标准输出与错误
来源：http://agl.xuanzx.com

cmd > out.log 2>&1
来源：http://qqa.yonumen.top

[R40] 追加写日志
来源：http://dzb.yuanzhike.top

echo "log" >> out.log
来源：http://bpx.yj20258.top

[R41] 丢弃输出
来源：http://oxl.jlsjyb.cn

cmd >/dev/null 2>&1
来源：http://nqv.fengsongda.top

[R42] 输入重定向
来源：http://wah.yj202588.top

wc -l < a.txt
来源：http://idm.yueranfly.top

[R43] 按名字查找文件
来源：http://eqs.yongpay.top

find . -name "*.log" -type f
来源：http://nqh.xuanzx.com

[R44] 按修改时间查找
来源：http://vke.daxiang520.top

find . -mtime -7 -type f
来源：http://het.guowangkeji.top

[R45] 批量删除
来源：http://yob.xylfe.cn

find . -name "*.tmp" -delete
来源：http://qhw.c1oappe.top

[R46] 递归替换文件内容
来源：http://uby.sxryk.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lom.316326.xyz

[R47] sed 单行替换
来源：http://uya.c1oappe.top

sed -i 's/foo/bar/g' a.txt
来源：http://wtc.ctjpmb.com

[R48] awk 取指定列
来源：http://wpv.zhoulong.xyz

awk '{print $1, $3}' a.txt
来源：http://umu.hammf.cn

[R49] awk 带条件
来源：http://paz.zdqjudy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xki.cucudq.cn

[R50] awk 求和
来源：http://pen.guowangkeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://stb.jyoumei.cn

[R51] 排序去重取前几
来源：http://kpp.sysykeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://atj.pycfn.com

[R52] 统计行数
来源：http://hew.shzxlz.cn

wc -l a.txt
来源：http://dcb.hcnkem.com

[R53] 查看文件头与实时尾
来源：http://huk.hfpthk.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xxw.meibo888.top

[R54] 比较两个文件
来源：http://syk.xingfuxueyuan.xyz

diff a.txt b.txt
来源：http://iul.xuanzx.com

[R55] 压缩与解压
来源：http://vjf.havefunace.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jcu.aizwys.cn

[R56] 远程拷贝
来源：http://iym.smart0.xyz

scp file user@host:/path/
来源：http://xmy.cucudq.cn

[R57] 远程执行命令
来源：http://jdi.yj20258.top

ssh user@host 'uptime'
来源：http://wjb.yanxiufei.cn

[R58] 下载文件
来源：http://yah.xuetiantiany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://erx.gaohongyu789.top

[R59] 发 POST JSON
来源：http://odu.316326.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tlm.yj202588.top

[R60] 只看 HTTP 状态码
来源：http://gai.chenjidiqi.icu

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://duh.shuidangran.top

[R61] 磁盘占用
来源：http://cfy.chenlongwang.top

df -h;  du -sh *
来源：http://akp.xuetiantiany.cn

[R62] 找最占空间的文件
来源：http://pmy.zhixingplan.top

du -ah . | sort -rh | head -10
来源：http://hbs.svipenyu.cn

[R63] 内存与进程
来源：http://gjf.tianlin.xyz

free -h;  ps aux | grep nginx
来源：http://vug.gzhubu.top

[R64] 结束进程
来源：http://fpx.guannengcc.top

kill -9 $(pgrep -f app.py)
来源：http://gks.fzhhl.top

[R65] 查看端口占用
来源：http://sdy.redwolf501.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kbh.daria6918.cn

[R66] 定时任务
来源：http://lso.guannengcc.top

crontab -e;  crontab -l
来源：http://tul.svipenyu.cn

[R67] 生成随机十六进制串
来源：http://vox.vqdsnc.cn

openssl rand -hex 16
来源：http://tha.xuetiantiany.cn

[R68] 计算文件校验值
来源：http://jok.fengsongda.top

sha256sum a.txt;  md5sum a.txt
来源：http://ldz.zhengqikj.top

[R69] 生成随机密码
来源：http://zuq.smart0.xyz


<!-- 参考信息 -->