代发 wailian999

);
来源：http://qyg.shzxlz.cn

[Q03] 增加列
来源：http://fmy.sysykeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xzm.daxiang520.top

[Q04] 修改列类型
来源：http://kdn.yonumen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gtx.sjlbkw.cn

[Q05] 重命名列
来源：http://xxa.dianchejie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vmy.yj20258.top

[Q06] 删除列
来源：http://qof.quarkkingdee.top

ALTER TABLE users DROP COLUMN age;
来源：http://ddw.iojbl.cn

[Q07] 删除表
来源：http://fqf.yongpay.top

DROP TABLE IF EXISTS orders;
来源：http://mat.chenzaomai.com

[Q08] 创建普通索引
来源：http://rou.fehbvm.com

CREATE INDEX idx_users_email ON users(email);
来源：http://wye.yangfankeji.com

[Q09] 创建唯一索引
来源：http://hpj.havefunace.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://url.gotoacloud.top

[Q10] 插入单行
来源：http://sui.hesvh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vsf.fengsongda.top

[Q11] 一次插入多行
来源：http://ngs.meibo888.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mco.aizwys.cn

[Q12] 插入后取自增 ID
来源：http://kno.pycfn.com

INSERT INTO users (name) VALUES ('C');
来源：http://osi.andypj.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ggd.birdmap.top

[Q13] 忽略重复插入
来源：http://ouz.yvedp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ynu.ivvv.top

[Q14] 存在则更新（upsert）
来源：http://wyt.sjlbkw.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://itd.guowangkeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hdi.ppjwa.cn

[Q15] 查询全部
来源：http://vcv.fengsongda.top

SELECT * FROM users;
来源：http://awf.ctjpmb.com

[Q16] 查询指定列
来源：http://akw.pycfn.com

SELECT id, name FROM users;
来源：http://vpr.ydjk.org.cn

[Q17] 条件查询
来源：http://rqv.jiagoushi.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ksi.svipenyu.cn

[Q18] 模糊匹配
来源：http://pjp.hysaishi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ixs.sxryk.cn

[Q19] 范围查询
来源：http://bbw.hcnkem.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rre.gogol.net.cn

[Q20] IN 列表
来源：http://rzx.jqgufenzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cvi.jinqigfzy.top

[Q21] 空值判断
来源：http://pyy.jinqigufen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ujq.zhixingplan.top

[Q22] 排序
来源：http://bwr.sxryk.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nnc.9152youxi.cn

[Q23] 分页
来源：http://lle.guowangkeji.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hja.zdbjq.cn

[Q24] 去重
来源：http://rql.mhx1999.top

SELECT DISTINCT city FROM users;
来源：http://guj.sufxvd.cn

[Q25] 只取前 N 条
来源：http://sya.yvedp.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://piz.316326.xyz

[Q26] 计数
来源：http://cdq.feifeiyinyue.top

SELECT COUNT(*) FROM users;
来源：http://fzd.gzhubu.top

[Q27] 条件计数
来源：http://owz.hnxiangtu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://txt.feifeiyinyue.top

[Q28] 求和与平均
来源：http://utx.fengsongda.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hlg.ydjk.org.cn

[Q29] 最大最小值
来源：http://oxu.wangshuangyany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fov.zdqjudy.top

[Q30] 分组统计
来源：http://pko.zhengqikj.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nbh.cqqwz.cn

[Q31] 分组后过滤
来源：http://cyw.yfazqb.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vmw.shanyushiyangkeji.top

[Q32] 分组拼接字符串
来源：http://mqh.gaohongyu789.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ijy.zhijiandao.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gsk.ywan-chungtsiang.top

[Q33] 多列分组
来源：http://kso.bbcook.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kxp.tian-w.cn

[Q34] 每组取第一条
来源：http://epl.9152youxi.cn

SELECT * FROM (
来源：http://rmg.redwolf501.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qyu.jinghuilouyu.cn

) t WHERE rn = 1;
来源：http://sjz.hysaishi.cn

[Q35] 内连接
来源：http://wce.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zbo.vehdjk.com

[Q36] 左连接
来源：http://cvo.jqgfzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kuw.sjlbkw.cn

[Q37] 右连接
来源：http://shn.jiagoushi.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xfm.guowangkeji.top

[Q38] 全外连接（PostgreSQL）
来源：http://jbk.ydzc1.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rfe.jqgufenzy.top

[Q39] 自连接（查上下级）
来源：http://ajg.epnwcf.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://dra.hesvh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qpr.ivvv.top

[Q40] 交叉连接（笛卡尔积）
来源：http://gvb.yangfankeji.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tze.zhiwuduotai.top

[Q41] 多表连接
来源：http://nzh.fengsongda.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://huc.zycfv.cn

JOIN users u ON u.id = o.user_id
来源：http://mrt.hongshengwenyu.top

JOIN products p ON p.id = o.product_id;
来源：http://tut.yfazqb.com

[Q42] 连接条件附加过滤
来源：http://bbc.xziqi.cn

SELECT u.name, o.amount FROM users u
来源：http://cdb.xinyue.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gok.fanxiaobao.xyz

[Q43] 标量子查询
来源：http://qsr.yvedp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cbj.yfazqb.com

[Q44] IN 子查询
来源：http://ail.fehbvm.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ort.zhoulong.xyz

[Q45] EXISTS 判断存在
来源：http://sbu.hcnkem.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mvc.cqqwz.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vhk.cashguo.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dya.iojbl.cn

[Q47] 与平均值比较
来源：http://guh.wangshuangyany.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zxf.xingfuxueyuan.xyz

[Q48] CTE 公用表表达式
来源：http://tbm.nanxinkj.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://moh.cashguo.top

SELECT * FROM t WHERE c > 5;
来源：http://opj.jiagoushi.top

[Q49] 更新单行
来源：http://liz.gogol.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zos.daxiang520.top

[Q50] 批量更新
来源：http://ynl.wangdashe.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://alo.sjlbkw.cn

[Q51] 用子查询更新
来源：http://dax.chenjidiqi.icu

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://spi.pycfn.com

[Q52] 删除指定行
来源：http://uwu.zdqjudy.top

DELETE FROM users WHERE id = 10;
来源：http://vtg.yj20258888.top

[Q53] 按条件删除
来源：http://jht.pycfn.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://azz.yj202588.top

[Q54] 清空表
来源：http://weq.ybcxt.top

TRUNCATE TABLE logs;
来源：http://lyd.cheryme.top

[Q55] 排名（并列占位）
来源：http://rxc.hammf.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dnd.gotoacloud.top

[Q56] 密集排名（并列不占位）
来源：http://pzi.sjlbkw.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://okm.sufxvd.cn

[Q57] 行号
来源：http://xhs.zhengqikj.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qjv.feifeiyinyue.top

[Q58] 累计求和
来源：http://zjx.hnxiangtu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yfc.ppjwa.cn

[Q59] 分组内累计
来源：http://rdx.ywan-chungtsiang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zvt.jqgufenzy.top

[Q60] 取上一行 / 下一行
来源：http://byc.redwolf501.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://myg.mhx1999.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yxh.smart0.xyz

[Q61] 移动平均
来源：http://shr.tarul.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ntc.aibaodan.cn

[Q62] 分组占比
来源：http://emh.shangyingyoupin.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://teh.hongshengwenyu.top

[Q63] 开启事务
来源：http://ndm.havefunace.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tbb.sufxvd.cn

[Q64] 提交事务
来源：http://hbm.zhiwuduotai.top

COMMIT;
来源：http://vhs.cashguo.top

[Q65] 回滚事务
来源：http://poq.ywan-chungtsiang.top

ROLLBACK;
来源：http://wlh.zycfv.cn

[Q66] 行锁查询
来源：http://jou.hongshengwenyu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sff.shangyingyoupin.top

[Q67] 设置隔离级别
来源：http://czw.hywenlv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://viy.zhixingplan.top

[Q68] 保存点
来源：http://end.svipenyu.cn

SAVEPOINT sp1;
来源：http://nde.hnxiangtu.top

ROLLBACK TO sp1;
来源：http://itx.jianghu66.top

[Q69] 查看执行计划
来源：http://zko.andypj.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uum.bjfxy.top

[Q70] 更新统计信息
来源：http://juv.ctjpmb.com

ANALYZE TABLE users;
来源：http://sco.xuanzx.com

[Q71] 查看建表语句
来源：http://ldb.zhiwuduotai.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gve.jinghuilouyu.cn

[Q72] 查看索引
来源：http://hgw.jqgfzy.top

SHOW INDEX FROM users;
来源：http://fha.snrcjt.cn

[Q73] 查看表状态
来源：http://nit.yuanzhike.top

SHOW TABLE STATUS LIKE 'users';
来源：http://jac.haohaochexian.top

[Q74] 强制使用索引
来源：http://dvu.cdnleiting.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://obu.hammf.cn

[Q75] 日期格式化
来源：http://pro.zhijiandao.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gky.jlsjyb.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pjs.chenzaomai.com

[Q76] 按天统计
来源：http://onv.tian-w.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rtz.ydjk.org.cn

[Q77] 时间加减
来源：http://dzp.yueranfly.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qkz.chenjidiqi.icu

[Q78] 当前时间
来源：http://iha.jinqigfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mvs.sweek.top

[Q79] 字符串拼接
来源：http://hsr.guannengcc.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ntw.c1oappe.top

[Q80] 字符串截取
来源：http://ire.fengsongda.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xsp.chenzaomai.com

[Q81] 字符串替换
来源：http://hqy.ppjwa.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lgj.meibo888.top

[Q82] 字符长度与字节长度
来源：http://yaw.iojbl.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fhp.jinghuilouyu.cn

[Q83] 大小写转换
来源：http://yda.tarul.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pmx.aizwys.cn

[Q84] 去除首尾空格
来源：http://zjo.shangyingyoupin.top

SELECT TRIM(name) FROM users;
来源：http://hng.wangshuangyany.cn

[Q85] 数值取整
来源：http://yvm.c1oappe.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lfk.vqdsnc.cn

[Q86] 读取 JSON 字段
来源：http://sib.hfpthk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://aeg.zhiwuduotai.top

[Q87] JSON 字段做条件
来源：http://mxj.cashguo.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vjl.meibo888.top

[Q88] 行转列（条件聚合）
来源：http://gxx.iojbl.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vyl.jqgfzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wqa.zhijiandao.cn

[Q89] 判断表是否存在
来源：http://hfr.zdbjq.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://maw.52xcode.cn

[Q90] 生成序号列
来源：http://exx.gzhubu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://poh.vqdsnc.cn

================================================================================
来源：http://ogp.chenzaomai.com

R. Bash 专题
来源：http://cbs.sxryk.cn

================================================================================
来源：http://omd.zhongyouzk.top

[R01] shebang 与严格模式
来源：http://jyc.jinqigfzy.top

#!/usr/bin/env bash
来源：http://vdb.jinghuilouyu.cn

set -euo pipefail
来源：http://bqr.aibaodan.cn

[R02] 变量赋值与使用
来源：http://ypq.ywan-chungtsiang.top

name="Tom"; echo "$name"
来源：http://ogw.yongpay.top

[R03] 只读变量
来源：http://leb.jqgfzy.top

readonly PI=3.14
来源：http://pfo.dashuyun.cn

[R04] 位置参数
来源：http://npw.gogol.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eiy.hnxiangtu.top

[R05] 参数默认值
来源：http://jnv.daxiang520.top

name="${1:-default}"
来源：http://mki.zhixingplan.top

[R06] 判断命令是否存在
来源：http://xbq.jianghu66.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cgc.xuetiantiany.cn

[R07] if 判断文件
来源：http://fwp.tianlin.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sji.birdmap.top

[R08] 数值比较
来源：http://qko.daria6918.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mto.zhengqikj.top

[R09] 字符串比较
来源：http://pja.ctjpmb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dcs.xylfe.cn

[R10] 正则匹配
来源：http://jen.xingfuxueyuan.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vgp.mhx1999.top

[R11] case 多分支
来源：http://kjq.quarkkingdee.top

case "$1" in
来源：http://gwa.svipenyu.cn

start) echo "启动" ;;
来源：http://ydk.tian-w.cn

stop)  echo "停止" ;;
来源：http://obo.yj20258.top

*)     echo "未知命令" ;;
来源：http://pbj.hysaishi.cn

esac
来源：http://cue.guowangkeji.top

[R12] for 遍历文件
来源：http://nau.nanxinkj.top

for f in *.txt; do echo "$f"; done
来源：http://jiy.jianghu66.top

[R13] for 计数循环
来源：http://uyo.sysykeji.top

for i in {1..10}; do echo "$i"; done
来源：http://fgd.zhijiandao.cn

[R14] C 风格 for
来源：http://cra.ybcxt.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://htj.guannengcc.top

[R15] while 逐行读文件
来源：http://xfn.fehbvm.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jvo.hesvh.cn

[R16] until 等待条件
来源：http://ktm.jlsjyb.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sml.haohaochexian.top

[R17] 数组定义与取值
来源：http://kjl.ywan-chungtsiang.top

arr=(a b c); echo "${arr[0]}"
来源：http://uau.wangshuangyany.cn

[R18] 遍历数组
来源：http://ovn.cheryme.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ybx.yongpay.top

[R19] 数组长度
来源：http://obe.birdmap.top

echo "${#arr[@]}"
来源：http://mgo.fktsv.cn

[R20] 关联数组（字典）
来源：http://taj.mhx1999.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://swg.jinyuanbaomall.cn

[R21] 字符串长度
来源：http://iiz.c1oappe.top

echo "${#s}"
来源：http://dqj.zycfv.cn

[R22] 截取子串
来源：http://zth.dashuyun.cn

echo "${s:0:5}"
来源：http://hwh.shangyingyoupin.top

[R23] 字符串替换
来源：http://otm.fengsongda.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xfy.yongpay.top

[R24] 大小写转换
来源：http://nhb.shangyingyoupin.top

echo "${s^^}"; echo "${s,,}"
来源：http://elt.shanyushiyangkeji.top

[R25] 去后缀 / 去前缀
来源：http://fkv.nanxuanxn.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://xds.wangshuangyany.cn

[R26] 命令替换
来源：http://jcu.cucudq.cn

now=$(date +%F); echo "$now"
来源：http://exr.ybcxt.top

[R27] 算术展开
来源：http://kac.shuidangran.top

echo $((1 + 2 * 3))
来源：http://hac.gzhubu.top

[R28] 浮点运算
来源：http://eyz.tian-w.cn

echo "scale=2; 10/3" | bc
来源：http://vab.havefunace.top

[R29] 定义函数
来源：http://nxm.ybcxt.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://udo.aizwys.cn

[R30] 函数返回状态码
来源：http://not.aibaodan.cn

f() { return 0; }; f || echo "失败了"
来源：http://tfo.jinqigufen.top

[R31] 局部变量
来源：http://ebm.yuxming.cn

f() { local x=1; echo "$x"; }
来源：http://zbn.tarul.cn

[R32] 参数个数校验
来源：http://gqv.nwbrower.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gmv.hesvh.cn

[R33] 捕获错误并提示行号
来源：http://kou.fzhhl.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uhq.hnxiangtu.top

[R34] 退出时清理
来源：http://pzo.jinghuilouyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wiu.guowangkeji.top

[R35] 后台执行并等待
来源：http://xdr.ydzc1.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xmp.chenlongwang.top

[R36] 并发执行多个任务
来源：http://hps.epnwcf.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nha.jqgfzy.top

[R37] 把输出赋给变量
来源：http://sgr.nanxuanxn.top

files=$(ls -1)
来源：http://uhw.aibaodan.cn

[R38] 管道串联
来源：http://duv.aizwys.cn

cat a.txt | grep -i error | wc -l
来源：http://anh.xuanzx.com

[R39] 重定向标准输出与错误
来源：http://rkf.ybcxt.top

cmd > out.log 2>&1
来源：http://owi.epnwcf.com

[R40] 追加写日志
来源：http://qdw.xylfe.cn

echo "log" >> out.log
来源：http://aij.hongshengwenyu.top

[R41] 丢弃输出
来源：http://eqq.ydzc1.top

cmd >/dev/null 2>&1
来源：http://tgq.yfazqb.com

[R42] 输入重定向
来源：http://ubc.cheryme.top

wc -l < a.txt
来源：http://bkd.ppjwa.cn

[R43] 按名字查找文件
来源：http://ajx.yvedp.cn

find . -name "*.log" -type f
来源：http://ipf.quarkkingdee.top

[R44] 按修改时间查找
来源：http://brj.52xcode.cn

find . -mtime -7 -type f
来源：http://ghb.zhengqikj.top

[R45] 批量删除
来源：http://wsx.xylfe.cn

find . -name "*.tmp" -delete
来源：http://chv.pengpengdd.cyou

[R46] 递归替换文件内容
来源：http://dix.zdqjudy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tvi.fanxiaobao.xyz

[R47] sed 单行替换
来源：http://pgw.sweek.top

sed -i 's/foo/bar/g' a.txt
来源：http://zxu.chenjidiqi.icu

[R48] awk 取指定列
来源：http://tqi.birdmap.top

awk '{print $1, $3}' a.txt
来源：http://dfv.shuidangran.top

[R49] awk 带条件
来源：http://pym.haohaochexian.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nhc.52xcode.cn

[R50] awk 求和
来源：http://gie.sufxvd.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dkl.tian-w.cn

[R51] 排序去重取前几
来源：http://puv.meibo888.top


<!-- 参考信息 -->