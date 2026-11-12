代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uui.vqdsnc.cn

);
来源：http://sdd.redwolf501.top

[Q02] 创建带外键的表
来源：http://gny.cashguo.top

CREATE TABLE orders (
来源：http://jqr.ywan-chungtsiang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ful.yfazqb.com

user_id INT NOT NULL,
来源：http://mfe.mhx1999.top

amount DECIMAL(10, 2),
来源：http://uqk.mhx1999.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jva.chenjidiqi.icu

);
来源：http://qak.wangshuangyany.cn

[Q03] 增加列
来源：http://omp.epnwcf.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sqs.shuidangran.top

[Q04] 修改列类型
来源：http://kun.yuanzhike.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uzu.yueranfly.top

[Q05] 重命名列
来源：http://wge.hnxiangtu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xqw.c1oappe.top

[Q06] 删除列
来源：http://zmn.xinyue.icu

ALTER TABLE users DROP COLUMN age;
来源：http://hak.pycfn.com

[Q07] 删除表
来源：http://uja.jianghu66.top

DROP TABLE IF EXISTS orders;
来源：http://hba.xylfe.cn

[Q08] 创建普通索引
来源：http://gmb.pengpengdd.cyou

CREATE INDEX idx_users_email ON users(email);
来源：http://rfh.ydjk.org.cn

[Q09] 创建唯一索引
来源：http://iwx.52xcode.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pla.316326.xyz

[Q10] 插入单行
来源：http://dhf.hcnkem.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gmv.sjlbkw.cn

[Q11] 一次插入多行
来源：http://kvk.haohaochexian.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lzd.hnxiangtu.top

[Q12] 插入后取自增 ID
来源：http://ubo.pengpengdd.cyou

INSERT INTO users (name) VALUES ('C');
来源：http://wiw.yj20258.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vcc.gotoacloud.top

[Q13] 忽略重复插入
来源：http://wyd.yvedp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fyo.xinyue.icu

[Q14] 存在则更新（upsert）
来源：http://zhn.hysaishi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://elk.smart0.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://euk.epnwcf.com

[Q15] 查询全部
来源：http://jgi.gaohongyu789.top

SELECT * FROM users;
来源：http://klv.svipenyu.cn

[Q16] 查询指定列
来源：http://jvf.xuanzx.com

SELECT id, name FROM users;
来源：http://pex.yj20258.top

[Q17] 条件查询
来源：http://deq.iojbl.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xfz.cheryme.top

[Q18] 模糊匹配
来源：http://wum.meibo888.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rhg.chenzaomai.com

[Q19] 范围查询
来源：http://tcs.ctjpmb.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xiw.fktsv.cn

[Q20] IN 列表
来源：http://tla.andypj.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dyf.daria6918.cn

[Q21] 空值判断
来源：http://oow.xylfe.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qql.svipenyu.cn

[Q22] 排序
来源：http://vkh.yj20258.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yjq.sjlbkw.cn

[Q23] 分页
来源：http://ldt.jinghuilouyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uvc.andypj.xyz

[Q24] 去重
来源：http://hir.sufxvd.cn

SELECT DISTINCT city FROM users;
来源：http://hsc.smart0.xyz

[Q25] 只取前 N 条
来源：http://ppc.0kj1m.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yyc.ppjwa.cn

[Q26] 计数
来源：http://ulj.havefunace.top

SELECT COUNT(*) FROM users;
来源：http://idi.vehdjk.com

[Q27] 条件计数
来源：http://sig.hesvh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zck.iojbl.cn

[Q28] 求和与平均
来源：http://xge.jyoumei.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vwl.gaohongyu789.top

[Q29] 最大最小值
来源：http://mmt.xziqi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://inp.bbcook.cn

[Q30] 分组统计
来源：http://uwn.fehbvm.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bvb.svipenyu.cn

[Q31] 分组后过滤
来源：http://kfg.cdnleiting.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ngq.bjfxy.top

[Q32] 分组拼接字符串
来源：http://swd.cucudq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ihf.ywan-chungtsiang.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vcu.dashuyun.cn

[Q33] 多列分组
来源：http://qnu.yj20258888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ufc.yfazqb.com

[Q34] 每组取第一条
来源：http://hto.jinyuanbaomall.cn

SELECT * FROM (
来源：http://fbz.tanke756.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://okx.feifeiyinyue.top

) t WHERE rn = 1;
来源：http://xgw.jinyuanbaomall.cn

[Q35] 内连接
来源：http://ehz.gaohongyu789.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dah.aizwys.cn

[Q36] 左连接
来源：http://auz.mhx1999.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://huu.sufxvd.cn

[Q37] 右连接
来源：http://eou.xingfuxueyuan.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://akh.jianghu66.top

[Q38] 全外连接（PostgreSQL）
来源：http://pwt.ydjk.org.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wqv.dianchejie.cn

[Q39] 自连接（查上下级）
来源：http://lqb.mhx1999.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://lvh.fzhhl.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yyq.chenlongwang.top

[Q40] 交叉连接（笛卡尔积）
来源：http://bne.9152youxi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://prs.hywenlv.cn

[Q41] 多表连接
来源：http://avq.gotoacloud.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://oug.vqdsnc.cn

JOIN users u ON u.id = o.user_id
来源：http://mky.yj20258.top

JOIN products p ON p.id = o.product_id;
来源：http://xpp.ydzc1.top

[Q42] 连接条件附加过滤
来源：http://gep.pycfn.com

SELECT u.name, o.amount FROM users u
来源：http://bxg.shuidangran.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uut.guannengcc.top

[Q43] 标量子查询
来源：http://ugo.tarul.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://beo.kuanghao11.cn

[Q44] IN 子查询
来源：http://ydw.cdnleiting.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wzh.hcnkem.com

[Q45] EXISTS 判断存在
来源：http://zjx.guowangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zam.chenzaomai.com

[Q46] NOT EXISTS 判断不存在
来源：http://hus.yj202588.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qxb.dashuyun.cn

[Q47] 与平均值比较
来源：http://ftt.redwolf501.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fbo.jqgfzy.top

[Q48] CTE 公用表表达式
来源：http://ahb.xuanzx.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sjw.aizwys.cn

SELECT * FROM t WHERE c > 5;
来源：http://xjf.hcnkem.com

[Q49] 更新单行
来源：http://hlv.hnxiangtu.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cst.hnxiangtu.top

[Q50] 批量更新
来源：http://kez.zdbjq.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://emb.fehbvm.com

[Q51] 用子查询更新
来源：http://vbu.sufxvd.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://abc.jinyuanbaomall.cn

[Q52] 删除指定行
来源：http://ogj.tianlin.xyz

DELETE FROM users WHERE id = 10;
来源：http://eaa.hammf.cn

[Q53] 按条件删除
来源：http://ajb.xylfe.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://asf.hnqzz.top

[Q54] 清空表
来源：http://emf.xingfuxueyuan.xyz

TRUNCATE TABLE logs;
来源：http://dij.feifeiyinyue.top

[Q55] 排名（并列占位）
来源：http://efo.zhixingplan.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://usx.0kj1m.cn

[Q56] 密集排名（并列不占位）
来源：http://cwu.0kj1m.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wea.zhoulong.xyz

[Q57] 行号
来源：http://ykd.cdnleiting.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ebr.havefunace.top

[Q58] 累计求和
来源：http://jlo.cheryme.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cxk.yvedp.cn

[Q59] 分组内累计
来源：http://kqa.zhixingplan.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ain.chenzaomai.com

[Q60] 取上一行 / 下一行
来源：http://ayf.ybcxt.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mlu.hesvh.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ytq.nanxuanxn.top

[Q61] 移动平均
来源：http://mml.ctjpmb.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zdh.yuxming.cn

[Q62] 分组占比
来源：http://xge.yangfankeji.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ils.yfazqb.com

[Q63] 开启事务
来源：http://pnr.xinyue.icu

START TRANSACTION;                -- 或 BEGIN
来源：http://jla.hywenlv.cn

[Q64] 提交事务
来源：http://ipb.shanyushiyangtech.top

COMMIT;
来源：http://oks.hcnkem.com

[Q65] 回滚事务
来源：http://rll.xuanzx.com

ROLLBACK;
来源：http://lip.fengsongda.top

[Q66] 行锁查询
来源：http://vzm.zdqjudy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://miz.snrcjt.cn

[Q67] 设置隔离级别
来源：http://pna.fktsv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nvr.xingfuxueyuan.xyz

[Q68] 保存点
来源：http://hxp.chenzaomai.com

SAVEPOINT sp1;
来源：http://erl.daria6918.cn

ROLLBACK TO sp1;
来源：http://yrl.feifeiyinyue.top

[Q69] 查看执行计划
来源：http://kgc.dashuyun.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tyc.yj202588.top

[Q70] 更新统计信息
来源：http://xsa.zdqjudy.top

ANALYZE TABLE users;
来源：http://wxt.gotoacloud.top

[Q71] 查看建表语句
来源：http://pxo.yj20258.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://knu.0kj1m.cn

[Q72] 查看索引
来源：http://evo.epnwcf.com

SHOW INDEX FROM users;
来源：http://mni.xuanzx.com

[Q73] 查看表状态
来源：http://hrh.xingfuxueyuan.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://ppb.haohaochexian.top

[Q74] 强制使用索引
来源：http://ddh.0kj1m.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mfi.shanyushiyangtech.top

[Q75] 日期格式化
来源：http://oza.gotoacloud.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fpk.jinqigufen.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bkr.hfpthk.cn

[Q76] 按天统计
来源：http://lpx.yfazqb.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mdf.zdqjudy.top

[Q77] 时间加减
来源：http://hzc.shanyushiyangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oak.shangyingyoupin.top

[Q78] 当前时间
来源：http://uju.birdmap.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rwt.daria6918.cn

[Q79] 字符串拼接
来源：http://qod.fktsv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yxr.fktsv.cn

[Q80] 字符串截取
来源：http://arx.9152youxi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hya.yangfankeji.com

[Q81] 字符串替换
来源：http://znm.shuidangran.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qjq.jinyuanbaomall.cn

[Q82] 字符长度与字节长度
来源：http://gvj.xinyue.icu

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cmn.yj20258888.top

[Q83] 大小写转换
来源：http://igw.316326.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pbo.shanyushiyangkeji.top

[Q84] 去除首尾空格
来源：http://url.pycfn.com

SELECT TRIM(name) FROM users;
来源：http://kkg.zhixingplan.top

[Q85] 数值取整
来源：http://dkm.quarkkingdee.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sdp.nwbrower.top

[Q86] 读取 JSON 字段
来源：http://zez.jyoumei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fxm.ywan-chungtsiang.top

[Q87] JSON 字段做条件
来源：http://ugn.jianghu66.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jid.cucudq.cn

[Q88] 行转列（条件聚合）
来源：http://ldt.yongpay.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bck.dashuyun.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ety.yonumen.top

[Q89] 判断表是否存在
来源：http://gxq.xuanzx.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xff.shangyingyoupin.top

[Q90] 生成序号列
来源：http://ppg.ybcxt.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rzh.fzhhl.top

================================================================================
来源：http://qnf.zhongyouzk.top

R. Bash 专题
来源：http://vse.mhx1999.top

================================================================================
来源：http://twz.yongpay.top

[R01] shebang 与严格模式
来源：http://xqb.gzhubu.top

#!/usr/bin/env bash
来源：http://wkq.jqgfzy.top

set -euo pipefail
来源：http://pzz.zhiwuduotai.top

[R02] 变量赋值与使用
来源：http://gry.yvedp.cn

name="Tom"; echo "$name"
来源：http://mto.sweek.top

[R03] 只读变量
来源：http://nea.uphjek.com

readonly PI=3.14
来源：http://tpb.ybcxt.top

[R04] 位置参数
来源：http://efj.52xcode.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nfh.hnxiangtu.top

[R05] 参数默认值
来源：http://nle.fengsongda.top

name="${1:-default}"
来源：http://bij.gzhubu.top

[R06] 判断命令是否存在
来源：http://rgm.ctjpmb.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mse.zhaomingkeji.xyz

[R07] if 判断文件
来源：http://snx.tianlin.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://awb.jinqigufen.top

[R08] 数值比较
来源：http://lrt.sufxvd.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kps.jlsjyb.cn

[R09] 字符串比较
来源：http://nba.sxryk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hvp.hcnkem.com

[R10] 正则匹配
来源：http://vgf.ydjk.org.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fel.cucudq.cn

[R11] case 多分支
来源：http://zbn.yvedp.cn

case "$1" in
来源：http://kte.sjlbkw.cn

start) echo "启动" ;;
来源：http://lzv.chenlongwang.top

stop)  echo "停止" ;;
来源：http://rgo.daxiang520.top

*)     echo "未知命令" ;;
来源：http://ttv.zhiwuduotai.top

esac
来源：http://aky.hesvh.cn

[R12] for 遍历文件
来源：http://dfs.chenjidiqi.icu

for f in *.txt; do echo "$f"; done
来源：http://sfc.shuidangran.top

[R13] for 计数循环
来源：http://eew.shanyushiyangkeji.top

for i in {1..10}; do echo "$i"; done
来源：http://qbk.kuanghao11.cn

[R14] C 风格 for
来源：http://rua.guannengcc.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lrv.kuanghao11.cn

[R15] while 逐行读文件
来源：http://eaw.jqgufenzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rzn.gzhubu.top

[R16] until 等待条件
来源：http://tsc.fehbvm.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kcw.yvedp.cn

[R17] 数组定义与取值
来源：http://yuf.ydzc1.top

arr=(a b c); echo "${arr[0]}"
来源：http://uah.xziqi.cn

[R18] 遍历数组
来源：http://xag.gzhubu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tgh.hnqzz.top

[R19] 数组长度
来源：http://xbg.hfpthk.cn

echo "${#arr[@]}"
来源：http://txg.chenlongwang.top

[R20] 关联数组（字典）
来源：http://pnt.nwbrower.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://phw.wangdashe.top

[R21] 字符串长度
来源：http://ypg.bbcook.cn

echo "${#s}"
来源：http://fln.hcnkem.com

[R22] 截取子串
来源：http://cwi.jinqigufen.top

echo "${s:0:5}"
来源：http://ter.chenzaomai.com

[R23] 字符串替换
来源：http://bnx.wangshuangyany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vdm.wangshuangyany.cn

[R24] 大小写转换
来源：http://ggl.tian-w.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uxw.chenlongwang.top

[R25] 去后缀 / 去前缀
来源：http://tmb.jiagoushi.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://six.tarul.cn

[R26] 命令替换
来源：http://lyf.yuanzhike.top

now=$(date +%F); echo "$now"
来源：http://prj.hesvh.cn

[R27] 算术展开
来源：http://wlw.yvedp.cn

echo $((1 + 2 * 3))
来源：http://dbm.zhixingplan.top

[R28] 浮点运算
来源：http://cvv.chenlongwang.top

echo "scale=2; 10/3" | bc
来源：http://urw.nanxinkj.top

[R29] 定义函数
来源：http://use.yongpay.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fmz.uphjek.com

[R30] 函数返回状态码
来源：http://jst.chenzaomai.com

f() { return 0; }; f || echo "失败了"
来源：http://dvo.haohaochexian.top

[R31] 局部变量
来源：http://iyx.xingfuxueyuan.xyz

f() { local x=1; echo "$x"; }
来源：http://piy.hywenlv.cn

[R32] 参数个数校验
来源：http://vjn.jiagoushi.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vzp.aizwys.cn

[R33] 捕获错误并提示行号
来源：http://dun.ywan-chungtsiang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yfd.shanyushiyangtech.top

[R34] 退出时清理
来源：http://eso.chenlongwang.top

trap 'rm -f "$tmp"' EXIT
来源：http://leb.redwolf501.top

[R35] 后台执行并等待
来源：http://xjp.jinyuanbaomall.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cid.nanxinkj.top

[R36] 并发执行多个任务
来源：http://rrx.fehbvm.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vvt.ivvv.top

[R37] 把输出赋给变量
来源：http://zlq.fehbvm.com

files=$(ls -1)
来源：http://ayg.yj20258.top

[R38] 管道串联
来源：http://clj.ybcxt.top

cat a.txt | grep -i error | wc -l
来源：http://toa.tarul.cn

[R39] 重定向标准输出与错误
来源：http://ywr.smart0.xyz

cmd > out.log 2>&1
来源：http://fcq.hesvh.cn

[R40] 追加写日志
来源：http://vbz.jinqigfzy.top

echo "log" >> out.log
来源：http://ixl.hammf.cn

[R41] 丢弃输出
来源：http://ulh.nanxuanxn.top

cmd >/dev/null 2>&1
来源：http://tod.daxiang520.top

[R42] 输入重定向
来源：http://otx.zhongyouzk.top

wc -l < a.txt
来源：http://jdg.sweek.top

[R43] 按名字查找文件
来源：http://vkt.cucudq.cn

find . -name "*.log" -type f
来源：http://bbr.snrcjt.cn

[R44] 按修改时间查找
来源：http://zjf.smart0.xyz

find . -mtime -7 -type f
来源：http://qop.haohaochexian.top

[R45] 批量删除
来源：http://tdx.quarkkingdee.top

find . -name "*.tmp" -delete
来源：http://kch.birdmap.top

[R46] 递归替换文件内容
来源：http://zpo.yj20258888.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zpe.hammf.cn

[R47] sed 单行替换
来源：http://txe.xinyue.icu


<!-- 参考信息 -->