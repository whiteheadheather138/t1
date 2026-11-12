代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://zkq.wangdashe.top

[Q07] 删除表
来源：http://geo.bbcook.cn

DROP TABLE IF EXISTS orders;
来源：http://wec.yj20258888.top

[Q08] 创建普通索引
来源：http://vdc.guannengcc.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ear.yfazqb.com

[Q09] 创建唯一索引
来源：http://rpy.shangyingyoupin.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nzu.cucudq.cn

[Q10] 插入单行
来源：http://zit.c1oappe.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://idh.guannengcc.top

[Q11] 一次插入多行
来源：http://pph.mhx1999.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mct.haohaochexian.top

[Q12] 插入后取自增 ID
来源：http://rxi.fktsv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://muq.zhijiandao.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://goy.zhoulong.xyz

[Q13] 忽略重复插入
来源：http://zmm.cqqwz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oou.shanyushiyangtech.top

[Q14] 存在则更新（upsert）
来源：http://ynu.hnxiangtu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nsq.cdnleiting.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uid.haohaochexian.top

[Q15] 查询全部
来源：http://oce.tianlin.xyz

SELECT * FROM users;
来源：http://ikc.jyoumei.cn

[Q16] 查询指定列
来源：http://prm.fzhhl.top

SELECT id, name FROM users;
来源：http://wbh.jinqigfzy.top

[Q17] 条件查询
来源：http://edu.jianghu66.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vid.fengsongda.top

[Q18] 模糊匹配
来源：http://qem.cdnleiting.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://otj.ctjpmb.com

[Q19] 范围查询
来源：http://vkj.9152youxi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pzf.havefunace.top

[Q20] IN 列表
来源：http://krr.hnxiangtu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ibi.birdmap.top

[Q21] 空值判断
来源：http://fbv.yj20258.top

SELECT * FROM users WHERE email IS NULL;
来源：http://vda.hysaishi.cn

[Q22] 排序
来源：http://qxb.jinqigfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://huj.ppjwa.cn

[Q23] 分页
来源：http://pph.jianghu66.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kci.redwolf501.top

[Q24] 去重
来源：http://rik.vehdjk.com

SELECT DISTINCT city FROM users;
来源：http://wes.hysaishi.cn

[Q25] 只取前 N 条
来源：http://vai.fktsv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fbz.jinqigufen.top

[Q26] 计数
来源：http://qgm.haohaochexian.top

SELECT COUNT(*) FROM users;
来源：http://lfw.jlsjyb.cn

[Q27] 条件计数
来源：http://wty.sjlbkw.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ctm.zhoulong.xyz

[Q28] 求和与平均
来源：http://vbw.ppjwa.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qjw.cdnleiting.top

[Q29] 最大最小值
来源：http://osl.cashguo.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://uwe.fehbvm.com

[Q30] 分组统计
来源：http://phq.yonumen.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dmq.sweek.top

[Q31] 分组后过滤
来源：http://oso.yj20258.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://egj.gotoacloud.top

[Q32] 分组拼接字符串
来源：http://ddp.cdnleiting.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yfg.gogol.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://umn.c1oappe.top

[Q33] 多列分组
来源：http://sdv.daria6918.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://knz.hammf.cn

[Q34] 每组取第一条
来源：http://bxf.ivvv.top

SELECT * FROM (
来源：http://zrm.shanyushiyangtech.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jrk.cheryme.top

) t WHERE rn = 1;
来源：http://kzt.guannengcc.top

[Q35] 内连接
来源：http://rnx.daria6918.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://knl.gaohongyu789.top

[Q36] 左连接
来源：http://lep.jqgufenzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pze.chenzaomai.com

[Q37] 右连接
来源：http://cjn.shzxlz.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yoh.jqgufenzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://syx.pycfn.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mrn.zhijiandao.cn

[Q39] 自连接（查上下级）
来源：http://pug.shangyingyoupin.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://bcg.sweek.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ase.havefunace.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zye.feifeiyinyue.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vtr.shzxlz.cn

[Q41] 多表连接
来源：http://ayj.wangshuangyany.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://nly.bjfxy.top

JOIN users u ON u.id = o.user_id
来源：http://ptb.yfazqb.com

JOIN products p ON p.id = o.product_id;
来源：http://gyi.guowangkeji.top

[Q42] 连接条件附加过滤
来源：http://brh.xuanzx.com

SELECT u.name, o.amount FROM users u
来源：http://mur.yuanzhike.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zdj.ivvv.top

[Q43] 标量子查询
来源：http://fwv.fanxiaobao.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pqc.zycfv.cn

[Q44] IN 子查询
来源：http://rdd.guowangkeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vpv.zycfv.cn

[Q45] EXISTS 判断存在
来源：http://jhk.jyoumei.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qav.zhiwuduotai.top

[Q46] NOT EXISTS 判断不存在
来源：http://gex.pengpengdd.cyou

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xju.zhongyouzk.top

[Q47] 与平均值比较
来源：http://vjv.yangfankeji.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qcj.xingfuxueyuan.xyz

[Q48] CTE 公用表表达式
来源：http://hcn.hnxiangtu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jak.chenlongwang.top

SELECT * FROM t WHERE c > 5;
来源：http://mgd.tianlin.xyz

[Q49] 更新单行
来源：http://rgz.ppjwa.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hja.jyoumei.cn

[Q50] 批量更新
来源：http://yxp.xuetiantiany.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gsd.sweek.top

[Q51] 用子查询更新
来源：http://xtb.bbcook.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://czi.fzhhl.top

[Q52] 删除指定行
来源：http://yxv.jiagoushi.top

DELETE FROM users WHERE id = 10;
来源：http://jsj.zhongyouzk.top

[Q53] 按条件删除
来源：http://gpy.kuanghao11.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bfw.fzhhl.top

[Q54] 清空表
来源：http://acv.ehwqpu.com

TRUNCATE TABLE logs;
来源：http://moj.zhongyouzk.top

[Q55] 排名（并列占位）
来源：http://ajv.meibo888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://iun.fzhhl.top

[Q56] 密集排名（并列不占位）
来源：http://kbj.mhx1999.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hlc.dashuyun.cn

[Q57] 行号
来源：http://vvv.tanke756.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://avc.hfpthk.cn

[Q58] 累计求和
来源：http://gqm.fzhhl.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://djn.sjlbkw.cn

[Q59] 分组内累计
来源：http://vey.chenlongwang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lla.yvedp.cn

[Q60] 取上一行 / 下一行
来源：http://ipy.jqgfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jdh.ywan-chungtsiang.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ydt.jinyuanbaomall.cn

[Q61] 移动平均
来源：http://uwb.tarul.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bdo.gaohongyu789.top

[Q62] 分组占比
来源：http://qka.shanyushiyangtech.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cft.jyoumei.cn

[Q63] 开启事务
来源：http://mvw.pengpengdd.cyou

START TRANSACTION;                -- 或 BEGIN
来源：http://mgd.jinqigufen.top

[Q64] 提交事务
来源：http://fyt.mhx1999.top

COMMIT;
来源：http://qhk.sxryk.cn

[Q65] 回滚事务
来源：http://ivz.havefunace.top

ROLLBACK;
来源：http://dbw.meibo888.top

[Q66] 行锁查询
来源：http://npi.ydjk.org.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ype.shangyingyoupin.top

[Q67] 设置隔离级别
来源：http://zyq.guowangkeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://whi.havefunace.top

[Q68] 保存点
来源：http://ldo.ydjk.org.cn

SAVEPOINT sp1;
来源：http://ldu.hesvh.cn

ROLLBACK TO sp1;
来源：http://qqi.zhongyouzk.top

[Q69] 查看执行计划
来源：http://ccw.uphjek.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kxk.sjlbkw.cn

[Q70] 更新统计信息
来源：http://bds.sxryk.cn

ANALYZE TABLE users;
来源：http://pze.hammf.cn

[Q71] 查看建表语句
来源：http://lti.aizwys.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://feh.cashguo.top

[Q72] 查看索引
来源：http://xmf.guannengcc.top

SHOW INDEX FROM users;
来源：http://jar.zhixingplan.top

[Q73] 查看表状态
来源：http://lfe.xylfe.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lcc.wangshuangyany.cn

[Q74] 强制使用索引
来源：http://rmx.zhijiandao.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ddg.0kj1m.cn

[Q75] 日期格式化
来源：http://eyw.gotoacloud.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wba.feifeiyinyue.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fsc.ydjk.org.cn

[Q76] 按天统计
来源：http://neq.dashuyun.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cyl.yvedp.cn

[Q77] 时间加减
来源：http://rph.xingfuxueyuan.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://loc.tanke756.top

[Q78] 当前时间
来源：http://wze.zhengqikj.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kxz.jinghuilouyu.cn

[Q79] 字符串拼接
来源：http://baj.xingfuxueyuan.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vdk.zhaomingkeji.xyz

[Q80] 字符串截取
来源：http://ddf.haohaochexian.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ctt.hongshengwenyu.top

[Q81] 字符串替换
来源：http://eai.kuanghao11.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mrl.daxiang520.top

[Q82] 字符长度与字节长度
来源：http://gni.9152youxi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tzq.hfpthk.cn

[Q83] 大小写转换
来源：http://ezp.wangshuangyany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hsg.gotoacloud.top

[Q84] 去除首尾空格
来源：http://muk.dashuyun.cn

SELECT TRIM(name) FROM users;
来源：http://ykb.chenlongwang.top

[Q85] 数值取整
来源：http://jox.tian-w.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yhq.yj202588.top

[Q86] 读取 JSON 字段
来源：http://vhg.meibo888.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xuq.nanxinkj.top

[Q87] JSON 字段做条件
来源：http://kwx.jlsjyb.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pic.xziqi.cn

[Q88] 行转列（条件聚合）
来源：http://kem.sxryk.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bst.zhijiandao.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://snc.sysykeji.top

[Q89] 判断表是否存在
来源：http://ikx.guowangkeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xtn.ctjpmb.com

[Q90] 生成序号列
来源：http://xle.guowangkeji.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://eri.fktsv.cn

================================================================================
来源：http://epm.andypj.xyz

R. Bash 专题
来源：http://zgn.shuidangran.top

================================================================================
来源：http://mbm.zdbjq.cn

[R01] shebang 与严格模式
来源：http://vwo.zhoulong.xyz

#!/usr/bin/env bash
来源：http://uwr.shangyingyoupin.top

set -euo pipefail
来源：http://rry.nanxuanxn.top

[R02] 变量赋值与使用
来源：http://rdh.hongshengwenyu.top

name="Tom"; echo "$name"
来源：http://aze.yuanzhike.top

[R03] 只读变量
来源：http://zgr.nanxinkj.top

readonly PI=3.14
来源：http://hrh.hnqzz.top

[R04] 位置参数
来源：http://kjk.ppjwa.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hcw.birdmap.top

[R05] 参数默认值
来源：http://lqc.yfazqb.com

name="${1:-default}"
来源：http://oal.gaohongyu789.top

[R06] 判断命令是否存在
来源：http://kwc.zhijiandao.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fvx.xuanzx.com

[R07] if 判断文件
来源：http://szs.shanyushiyangkeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mgt.sxryk.cn

[R08] 数值比较
来源：http://fez.uphjek.com

if (( a > b )); then echo "a 更大"; fi
来源：http://kdg.yj202588.top

[R09] 字符串比较
来源：http://fux.sjlbkw.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://aby.jqgfzy.top

[R10] 正则匹配
来源：http://vgt.ywan-chungtsiang.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ves.xziqi.cn

[R11] case 多分支
来源：http://yzz.c1oappe.top

case "$1" in
来源：http://omg.xziqi.cn

start) echo "启动" ;;
来源：http://ufc.hammf.cn

stop)  echo "停止" ;;
来源：http://rvy.hesvh.cn

*)     echo "未知命令" ;;
来源：http://xrp.zhixingplan.top

esac
来源：http://vko.epnwcf.com

[R12] for 遍历文件
来源：http://vry.guannengcc.top

for f in *.txt; do echo "$f"; done
来源：http://xle.daria6918.cn

[R13] for 计数循环
来源：http://sbf.cdnleiting.top

for i in {1..10}; do echo "$i"; done
来源：http://ewk.sweek.top

[R14] C 风格 for
来源：http://qhp.jiagoushi.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://byp.pengpengdd.cyou

[R15] while 逐行读文件
来源：http://xsl.bbcook.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ulp.hnqzz.top

[R16] until 等待条件
来源：http://apn.wangshuangyany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hdh.gotoacloud.top

[R17] 数组定义与取值
来源：http://pnr.jinghuilouyu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nwt.ybcxt.top

[R18] 遍历数组
来源：http://noy.hesvh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://doa.jinyuanbaomall.cn

[R19] 数组长度
来源：http://ltm.feifeiyinyue.top

echo "${#arr[@]}"
来源：http://lss.haohaochexian.top

[R20] 关联数组（字典）
来源：http://vuq.chenjidiqi.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mxq.epnwcf.com

[R21] 字符串长度
来源：http://zdb.yfazqb.com

echo "${#s}"
来源：http://waj.cheryme.top

[R22] 截取子串
来源：http://hlg.uphjek.com

echo "${s:0:5}"
来源：http://xpk.bjfxy.top

[R23] 字符串替换
来源：http://xzc.jianghu66.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kdc.yanxiufei.cn

[R24] 大小写转换
来源：http://kil.guannengcc.top

echo "${s^^}"; echo "${s,,}"
来源：http://cix.uphjek.com

[R25] 去后缀 / 去前缀
来源：http://lzp.shanyushiyangtech.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://aoy.zhaomingkeji.xyz

[R26] 命令替换
来源：http://rgj.hnxiangtu.top

now=$(date +%F); echo "$now"
来源：http://oys.bbcook.cn

[R27] 算术展开
来源：http://sap.gaohongyu789.top

echo $((1 + 2 * 3))
来源：http://yhv.jlsjyb.cn

[R28] 浮点运算
来源：http://azi.fktsv.cn

echo "scale=2; 10/3" | bc
来源：http://esv.nwbrower.top

[R29] 定义函数
来源：http://fal.tarul.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rql.zhiwuduotai.top

[R30] 函数返回状态码
来源：http://wnj.ydjk.org.cn

f() { return 0; }; f || echo "失败了"
来源：http://chv.ehwqpu.com

[R31] 局部变量
来源：http://naq.gaohongyu789.top

f() { local x=1; echo "$x"; }
来源：http://hxk.cucudq.cn

[R32] 参数个数校验
来源：http://snx.hysaishi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rab.zhiwuduotai.top

[R33] 捕获错误并提示行号
来源：http://gos.jinqigufen.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eca.316326.xyz

[R34] 退出时清理
来源：http://asr.yuxming.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qtu.nwbrower.top

[R35] 后台执行并等待
来源：http://typ.ydzc1.top

sleep 5 & pid=$!; wait "$pid"
来源：http://rxl.shangyingyoupin.top

[R36] 并发执行多个任务
来源：http://ylx.jiagoushi.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mfk.birdmap.top

[R37] 把输出赋给变量
来源：http://kwg.jinqigfzy.top

files=$(ls -1)
来源：http://cep.cheryme.top

[R38] 管道串联
来源：http://anc.dashuyun.cn

cat a.txt | grep -i error | wc -l
来源：http://gjc.zdqjudy.top

[R39] 重定向标准输出与错误
来源：http://yev.gzhubu.top

cmd > out.log 2>&1
来源：http://fcr.316326.xyz

[R40] 追加写日志
来源：http://osb.jinqigfzy.top

echo "log" >> out.log
来源：http://unz.birdmap.top

[R41] 丢弃输出
来源：http://tcq.zhijiandao.cn

cmd >/dev/null 2>&1
来源：http://dbn.ybcxt.top

[R42] 输入重定向
来源：http://oyq.yvedp.cn

wc -l < a.txt
来源：http://gte.haohaochexian.top

[R43] 按名字查找文件
来源：http://foh.jiagoushi.top

find . -name "*.log" -type f
来源：http://wcp.gotoacloud.top

[R44] 按修改时间查找
来源：http://iqw.guannengcc.top

find . -mtime -7 -type f
来源：http://bwb.aibaodan.cn

[R45] 批量删除
来源：http://ghf.yuanzhike.top

find . -name "*.tmp" -delete
来源：http://qgx.jlsjyb.cn

[R46] 递归替换文件内容
来源：http://rui.tian-w.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://agw.cheryme.top

[R47] sed 单行替换
来源：http://dmm.bbcook.cn

sed -i 's/foo/bar/g' a.txt
来源：http://czr.316326.xyz

[R48] awk 取指定列
来源：http://dab.316326.xyz

awk '{print $1, $3}' a.txt
来源：http://hhx.yvedp.cn

[R49] awk 带条件
来源：http://ews.pycfn.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dux.nanxinkj.top

[R50] awk 求和
来源：http://mgn.zhengqikj.top

awk '{s += $2} END {print s}' a.txt
来源：http://bzr.sweek.top

[R51] 排序去重取前几
来源：http://ehv.zycfv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hkm.zhoulong.xyz

[R52] 统计行数
来源：http://lbb.pycfn.com

wc -l a.txt
来源：http://jtu.nanxinkj.top

[R53] 查看文件头与实时尾
来源：http://bcv.tarul.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fbl.cashguo.top

[R54] 比较两个文件
来源：http://ywv.ydjk.org.cn

diff a.txt b.txt
来源：http://ldp.xingfuxueyuan.xyz

[R55] 压缩与解压
来源：http://lyd.ydjk.org.cn


<!-- 参考信息 -->