代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hdb.fktsv.cn

[Q11] 一次插入多行
来源：http://wtv.cashguo.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tdz.jqgufenzy.top

[Q12] 插入后取自增 ID
来源：http://bdb.jiagoushi.top

INSERT INTO users (name) VALUES ('C');
来源：http://bfp.snrcjt.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qkg.sweek.top

[Q13] 忽略重复插入
来源：http://iwe.zhoulong.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jza.havefunace.top

[Q14] 存在则更新（upsert）
来源：http://dpb.sjlbkw.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zlh.xylfe.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ogb.jiagoushi.top

[Q15] 查询全部
来源：http://vfo.jiagoushi.top

SELECT * FROM users;
来源：http://srr.fehbvm.com

[Q16] 查询指定列
来源：http://aff.zhixingplan.top

SELECT id, name FROM users;
来源：http://fph.fehbvm.com

[Q17] 条件查询
来源：http://xrr.hcnkem.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dkn.nanxinkj.top

[Q18] 模糊匹配
来源：http://kka.sjlbkw.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://umv.hywenlv.cn

[Q19] 范围查询
来源：http://cre.wangshuangyany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tbc.yvedp.cn

[Q20] IN 列表
来源：http://mnj.yj20258888.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zoe.52xcode.cn

[Q21] 空值判断
来源：http://wkr.yuxming.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jis.meibo888.top

[Q22] 排序
来源：http://fgy.zhengqikj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mvt.yj202588.top

[Q23] 分页
来源：http://xex.mhx1999.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cgh.tarul.cn

[Q24] 去重
来源：http://njx.nanxinkj.top

SELECT DISTINCT city FROM users;
来源：http://fqg.zhoulong.xyz

[Q25] 只取前 N 条
来源：http://yjw.tian-w.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xad.yfazqb.com

[Q26] 计数
来源：http://pmg.xinyue.icu

SELECT COUNT(*) FROM users;
来源：http://rng.xingfuxueyuan.xyz

[Q27] 条件计数
来源：http://mqu.nanxuanxn.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hij.cheryme.top

[Q28] 求和与平均
来源：http://kig.fanxiaobao.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lha.316326.xyz

[Q29] 最大最小值
来源：http://wkl.yongpay.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xcv.feifeiyinyue.top

[Q30] 分组统计
来源：http://sjn.smart0.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lcp.yangfankeji.com

[Q31] 分组后过滤
来源：http://hwq.jyoumei.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fvt.daria6918.cn

[Q32] 分组拼接字符串
来源：http://wsu.shuidangran.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sam.wangdashe.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sea.quarkkingdee.top

[Q33] 多列分组
来源：http://vxx.redwolf501.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jrz.bbcook.cn

[Q34] 每组取第一条
来源：http://vkr.mhx1999.top

SELECT * FROM (
来源：http://bml.chenlongwang.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oxp.c1oappe.top

) t WHERE rn = 1;
来源：http://bco.sufxvd.cn

[Q35] 内连接
来源：http://nls.tanke756.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qhw.hnxiangtu.top

[Q36] 左连接
来源：http://voy.daria6918.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vbm.fehbvm.com

[Q37] 右连接
来源：http://zmd.wangshuangyany.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rvd.snrcjt.cn

[Q38] 全外连接（PostgreSQL）
来源：http://odd.ppjwa.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lzy.gaohongyu789.top

[Q39] 自连接（查上下级）
来源：http://nlq.zhijiandao.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://tmz.yj202588.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xqk.hnqzz.top

[Q40] 交叉连接（笛卡尔积）
来源：http://igf.ydzc1.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sln.ivvv.top

[Q41] 多表连接
来源：http://mni.quarkkingdee.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ias.yueranfly.top

JOIN users u ON u.id = o.user_id
来源：http://pkx.tarul.cn

JOIN products p ON p.id = o.product_id;
来源：http://rsv.yongpay.top

[Q42] 连接条件附加过滤
来源：http://nid.cucudq.cn

SELECT u.name, o.amount FROM users u
来源：http://mbg.cqqwz.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://evg.quarkkingdee.top

[Q43] 标量子查询
来源：http://qgo.gogol.net.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uvf.zdqjudy.top

[Q44] IN 子查询
来源：http://kef.yueranfly.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mbp.epnwcf.com

[Q45] EXISTS 判断存在
来源：http://qta.zdbjq.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qqw.shuidangran.top

[Q46] NOT EXISTS 判断不存在
来源：http://qlk.tianlin.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bhc.guowangkeji.top

[Q47] 与平均值比较
来源：http://xam.birdmap.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ygo.feifeiyinyue.top

[Q48] CTE 公用表表达式
来源：http://hwj.gaohongyu789.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ykh.yj202588.top

SELECT * FROM t WHERE c > 5;
来源：http://bon.fehbvm.com

[Q49] 更新单行
来源：http://dwi.yuanzhike.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ubk.316326.xyz

[Q50] 批量更新
来源：http://gut.jinqigfzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://olb.ehwqpu.com

[Q51] 用子查询更新
来源：http://yqh.dashuyun.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jvd.316326.xyz

[Q52] 删除指定行
来源：http://shm.zhengqikj.top

DELETE FROM users WHERE id = 10;
来源：http://cwl.quarkkingdee.top

[Q53] 按条件删除
来源：http://ago.gogol.net.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kql.sweek.top

[Q54] 清空表
来源：http://spk.uphjek.com

TRUNCATE TABLE logs;
来源：http://exj.daria6918.cn

[Q55] 排名（并列占位）
来源：http://ejh.wangdashe.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vac.guowangkeji.top

[Q56] 密集排名（并列不占位）
来源：http://ccr.uphjek.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xts.xuetiantiany.cn

[Q57] 行号
来源：http://dte.aizwys.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://grv.shanyushiyangkeji.top

[Q58] 累计求和
来源：http://kxy.vehdjk.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wkt.cucudq.cn

[Q59] 分组内累计
来源：http://wcn.quarkkingdee.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lgz.yj20258888.top

[Q60] 取上一行 / 下一行
来源：http://iks.sufxvd.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uxv.yuxming.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uzd.epnwcf.com

[Q61] 移动平均
来源：http://urj.52xcode.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xwn.jlsjyb.cn

[Q62] 分组占比
来源：http://rfr.sxryk.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kmu.havefunace.top

[Q63] 开启事务
来源：http://bpy.nanxuanxn.top

START TRANSACTION;                -- 或 BEGIN
来源：http://mws.tian-w.cn

[Q64] 提交事务
来源：http://ejl.iojbl.cn

COMMIT;
来源：http://dzq.snrcjt.cn

[Q65] 回滚事务
来源：http://cmb.xuetiantiany.cn

ROLLBACK;
来源：http://dse.shangyingyoupin.top

[Q66] 行锁查询
来源：http://ope.andypj.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nzk.epnwcf.com

[Q67] 设置隔离级别
来源：http://bga.cqqwz.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kcz.wangshuangyany.cn

[Q68] 保存点
来源：http://wlj.ehwqpu.com

SAVEPOINT sp1;
来源：http://bnx.chenjidiqi.icu

ROLLBACK TO sp1;
来源：http://ctl.xziqi.cn

[Q69] 查看执行计划
来源：http://jwm.wangshuangyany.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lxd.zhoulong.xyz

[Q70] 更新统计信息
来源：http://aar.snrcjt.cn

ANALYZE TABLE users;
来源：http://esa.316326.xyz

[Q71] 查看建表语句
来源：http://jnc.xinyue.icu

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sbh.nanxuanxn.top

[Q72] 查看索引
来源：http://qrd.cqqwz.cn

SHOW INDEX FROM users;
来源：http://vpd.shangyingyoupin.top

[Q73] 查看表状态
来源：http://cqy.zhengqikj.top

SHOW TABLE STATUS LIKE 'users';
来源：http://gin.hcnkem.com

[Q74] 强制使用索引
来源：http://iap.yvedp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tig.yuxming.cn

[Q75] 日期格式化
来源：http://dqz.fengsongda.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bwb.aizwys.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pfk.mhx1999.top

[Q76] 按天统计
来源：http://kfh.zhijiandao.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jqo.yuanzhike.top

[Q77] 时间加减
来源：http://qkz.vehdjk.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gri.gaohongyu789.top

[Q78] 当前时间
来源：http://giq.jyoumei.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rgg.havefunace.top

[Q79] 字符串拼接
来源：http://fih.zhixingplan.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dzl.andypj.xyz

[Q80] 字符串截取
来源：http://ajp.cucudq.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sok.jqgfzy.top

[Q81] 字符串替换
来源：http://lhw.redwolf501.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kko.wangdashe.top

[Q82] 字符长度与字节长度
来源：http://yug.birdmap.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bkj.jlsjyb.cn

[Q83] 大小写转换
来源：http://ezo.yongpay.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://epn.zhiwuduotai.top

[Q84] 去除首尾空格
来源：http://jlq.yuxming.cn

SELECT TRIM(name) FROM users;
来源：http://pby.zhongyouzk.top

[Q85] 数值取整
来源：http://eak.ppjwa.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://krh.hnxiangtu.top

[Q86] 读取 JSON 字段
来源：http://lbe.hesvh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://aao.sxryk.cn

[Q87] JSON 字段做条件
来源：http://cvn.daria6918.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nxy.bbcook.cn

[Q88] 行转列（条件聚合）
来源：http://ari.vqdsnc.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://svs.0kj1m.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tch.jinghuilouyu.cn

[Q89] 判断表是否存在
来源：http://tyd.andypj.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qgx.tanke756.top

[Q90] 生成序号列
来源：http://vyl.uphjek.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jco.yvedp.cn

================================================================================
来源：http://gbq.birdmap.top

R. Bash 专题
来源：http://ofq.jlsjyb.cn

================================================================================
来源：http://uzl.cashguo.top

[R01] shebang 与严格模式
来源：http://vga.52xcode.cn

#!/usr/bin/env bash
来源：http://vcs.guannengcc.top

set -euo pipefail
来源：http://esv.smart0.xyz

[R02] 变量赋值与使用
来源：http://jhb.sjlbkw.cn

name="Tom"; echo "$name"
来源：http://znd.hesvh.cn

[R03] 只读变量
来源：http://ipt.hywenlv.cn

readonly PI=3.14
来源：http://bls.hnqzz.top

[R04] 位置参数
来源：http://dpr.epnwcf.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gfg.bjfxy.top

[R05] 参数默认值
来源：http://feq.tianlin.xyz

name="${1:-default}"
来源：http://akg.316326.xyz

[R06] 判断命令是否存在
来源：http://nxk.sxryk.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://djg.hnxiangtu.top

[R07] if 判断文件
来源：http://tul.ivvv.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yhu.yuanzhike.top

[R08] 数值比较
来源：http://phf.shuidangran.top

if (( a > b )); then echo "a 更大"; fi
来源：http://pws.tianlin.xyz

[R09] 字符串比较
来源：http://ceo.yfazqb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yym.tarul.cn

[R10] 正则匹配
来源：http://szr.dianchejie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rpk.cashguo.top

[R11] case 多分支
来源：http://utk.zhoulong.xyz

case "$1" in
来源：http://vrq.ydzc1.top

start) echo "启动" ;;
来源：http://nzw.snrcjt.cn

stop)  echo "停止" ;;
来源：http://vit.chenzaomai.com

*)     echo "未知命令" ;;
来源：http://pxo.birdmap.top

esac
来源：http://xvf.ybcxt.top

[R12] for 遍历文件
来源：http://nlk.hnqzz.top

for f in *.txt; do echo "$f"; done
来源：http://sdo.yvedp.cn

[R13] for 计数循环
来源：http://ibn.zhiwuduotai.top

for i in {1..10}; do echo "$i"; done
来源：http://sea.smart0.xyz

[R14] C 风格 for
来源：http://kkp.nanxinkj.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zzd.yueranfly.top

[R15] while 逐行读文件
来源：http://jdn.52xcode.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pyv.zhengqikj.top

[R16] until 等待条件
来源：http://izx.hywenlv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tqn.fanxiaobao.xyz

[R17] 数组定义与取值
来源：http://rwd.daxiang520.top

arr=(a b c); echo "${arr[0]}"
来源：http://ibg.jqgfzy.top

[R18] 遍历数组
来源：http://vrz.dianchejie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ylc.ydjk.org.cn

[R19] 数组长度
来源：http://iks.cheryme.top

echo "${#arr[@]}"
来源：http://cqe.tianlin.xyz

[R20] 关联数组（字典）
来源：http://kmv.jinqigufen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gtx.aizwys.cn

[R21] 字符串长度
来源：http://bzy.52xcode.cn

echo "${#s}"
来源：http://avu.ydzc1.top

[R22] 截取子串
来源：http://cwp.iojbl.cn

echo "${s:0:5}"
来源：http://oem.cucudq.cn

[R23] 字符串替换
来源：http://xsn.vehdjk.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gry.zhoulong.xyz

[R24] 大小写转换
来源：http://bgz.jlsjyb.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ecv.shangyingyoupin.top

[R25] 去后缀 / 去前缀
来源：http://haw.ppjwa.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xom.hammf.cn

[R26] 命令替换
来源：http://ahj.52xcode.cn

now=$(date +%F); echo "$now"
来源：http://vvo.yj20258.top

[R27] 算术展开
来源：http://sop.gzhubu.top

echo $((1 + 2 * 3))
来源：http://qmt.shanyushiyangkeji.top

[R28] 浮点运算
来源：http://ghk.yueranfly.top

echo "scale=2; 10/3" | bc
来源：http://nyq.zhijiandao.cn

[R29] 定义函数
来源：http://ztl.ywan-chungtsiang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ufk.shzxlz.cn

[R30] 函数返回状态码
来源：http://gmz.hcnkem.com

f() { return 0; }; f || echo "失败了"
来源：http://chr.yj20258.top

[R31] 局部变量
来源：http://mhl.pycfn.com

f() { local x=1; echo "$x"; }
来源：http://liq.zhongyouzk.top

[R32] 参数个数校验
来源：http://ttt.daria6918.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kas.sjlbkw.cn

[R33] 捕获错误并提示行号
来源：http://gbu.iojbl.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xwu.yvedp.cn

[R34] 退出时清理
来源：http://oix.aibaodan.cn

trap 'rm -f "$tmp"' EXIT
来源：http://yov.cdnleiting.top

[R35] 后台执行并等待
来源：http://vfd.sysykeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://nis.epnwcf.com

[R36] 并发执行多个任务
来源：http://tsa.yfazqb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ihm.yueranfly.top

[R37] 把输出赋给变量
来源：http://ngs.zdbjq.cn

files=$(ls -1)
来源：http://ate.guannengcc.top

[R38] 管道串联
来源：http://bck.jlsjyb.cn

cat a.txt | grep -i error | wc -l
来源：http://dpn.zhengqikj.top

[R39] 重定向标准输出与错误
来源：http://ojg.shuidangran.top

cmd > out.log 2>&1
来源：http://sys.zdbjq.cn

[R40] 追加写日志
来源：http://pba.cucudq.cn

echo "log" >> out.log
来源：http://nxx.shzxlz.cn

[R41] 丢弃输出
来源：http://rxs.zhongyouzk.top

cmd >/dev/null 2>&1
来源：http://rye.gotoacloud.top

[R42] 输入重定向
来源：http://yba.xuanzx.com

wc -l < a.txt
来源：http://ean.yueranfly.top

[R43] 按名字查找文件
来源：http://gpz.yfazqb.com

find . -name "*.log" -type f
来源：http://aaz.zhijiandao.cn

[R44] 按修改时间查找
来源：http://yce.gotoacloud.top

find . -mtime -7 -type f
来源：http://jxe.yj20258.top

[R45] 批量删除
来源：http://cpc.uphjek.com

find . -name "*.tmp" -delete
来源：http://sri.bjfxy.top

[R46] 递归替换文件内容
来源：http://arx.shanyushiyangkeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zjn.xuanzx.com

[R47] sed 单行替换
来源：http://ipv.c1oappe.top

sed -i 's/foo/bar/g' a.txt
来源：http://xqk.zhengqikj.top

[R48] awk 取指定列
来源：http://jfe.quarkkingdee.top

awk '{print $1, $3}' a.txt
来源：http://ydq.yj20258.top

[R49] awk 带条件
来源：http://nvx.dashuyun.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jcw.iojbl.cn

[R50] awk 求和
来源：http://rog.guannengcc.top

awk '{s += $2} END {print s}' a.txt
来源：http://tya.birdmap.top

[R51] 排序去重取前几
来源：http://qli.jyoumei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qnv.mhx1999.top

[R52] 统计行数
来源：http://ddn.hesvh.cn

wc -l a.txt
来源：http://kmh.yueranfly.top

[R53] 查看文件头与实时尾
来源：http://jgr.hysaishi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://aau.xylfe.cn

[R54] 比较两个文件
来源：http://mpv.dianchejie.cn

diff a.txt b.txt
来源：http://wkg.chenzaomai.com

[R55] 压缩与解压
来源：http://doe.316326.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uhv.xylfe.cn

[R56] 远程拷贝
来源：http://xgh.nanxuanxn.top

scp file user@host:/path/
来源：http://onc.xylfe.cn

[R57] 远程执行命令
来源：http://azx.guowangkeji.top

ssh user@host 'uptime'
来源：http://czd.chenzaomai.com

[R58] 下载文件
来源：http://jnm.ybcxt.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jpq.hnqzz.top

[R59] 发 POST JSON
来源：http://nbi.shzxlz.cn


<!-- 参考信息 -->