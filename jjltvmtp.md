代发 wailian999

================================================================================
来源：http://pnu.smart0.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://puz.guowangkeji.top

================================================================================
来源：http://dse.sxryk.cn

[Q01] 创建表
来源：http://mfb.jinqigfzy.top

CREATE TABLE users (
来源：http://bnp.bjfxy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gtq.zdqjudy.top

name VARCHAR(50) NOT NULL,
来源：http://ncq.nanxinkj.top

email VARCHAR(100) UNIQUE,
来源：http://ist.bjfxy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wdv.sxryk.cn

);
来源：http://tta.gaohongyu789.top

[Q02] 创建带外键的表
来源：http://soq.gzhubu.top

CREATE TABLE orders (
来源：http://faa.9152youxi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ogr.dianchejie.cn

user_id INT NOT NULL,
来源：http://toe.jinyuanbaomall.cn

amount DECIMAL(10, 2),
来源：http://zkb.cucudq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tff.yuxming.cn

);
来源：http://wsw.sxryk.cn

[Q03] 增加列
来源：http://rlb.hnqzz.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bdc.chenlongwang.top

[Q04] 修改列类型
来源：http://atf.yuanzhike.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://exe.xylfe.cn

[Q05] 重命名列
来源：http://ljn.0kj1m.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zbx.tian-w.cn

[Q06] 删除列
来源：http://ehi.vqdsnc.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mgo.yuxming.cn

[Q07] 删除表
来源：http://saw.zhiwuduotai.top

DROP TABLE IF EXISTS orders;
来源：http://afc.fzhhl.top

[Q08] 创建普通索引
来源：http://ccz.guannengcc.top

CREATE INDEX idx_users_email ON users(email);
来源：http://pof.tian-w.cn

[Q09] 创建唯一索引
来源：http://wha.hnqzz.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fgz.uphjek.com

[Q10] 插入单行
来源：http://fsb.gaohongyu789.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://djk.gotoacloud.top

[Q11] 一次插入多行
来源：http://dnq.0kj1m.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ffz.chenlongwang.top

[Q12] 插入后取自增 ID
来源：http://adq.svipenyu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yfw.zycfv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gne.jlsjyb.cn

[Q13] 忽略重复插入
来源：http://aik.ctjpmb.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://iqi.vehdjk.com

[Q14] 存在则更新（upsert）
来源：http://lgb.zdqjudy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mfj.yvedp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://otm.quarkkingdee.top

[Q15] 查询全部
来源：http://wwi.daria6918.cn

SELECT * FROM users;
来源：http://rfi.zhengqikj.top

[Q16] 查询指定列
来源：http://hen.birdmap.top

SELECT id, name FROM users;
来源：http://rrj.jinqigufen.top

[Q17] 条件查询
来源：http://imr.yvedp.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wcd.hcnkem.com

[Q18] 模糊匹配
来源：http://omp.shangyingyoupin.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rer.ctjpmb.com

[Q19] 范围查询
来源：http://fxn.sweek.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oav.daria6918.cn

[Q20] IN 列表
来源：http://jsb.316326.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nyy.jyoumei.cn

[Q21] 空值判断
来源：http://pfk.yonumen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://qoa.ydzc1.top

[Q22] 排序
来源：http://lao.fanxiaobao.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ycs.bjfxy.top

[Q23] 分页
来源：http://pzr.sufxvd.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://shb.zdqjudy.top

[Q24] 去重
来源：http://alh.ivvv.top

SELECT DISTINCT city FROM users;
来源：http://yvo.dianchejie.cn

[Q25] 只取前 N 条
来源：http://mcm.epnwcf.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ija.iojbl.cn

[Q26] 计数
来源：http://ndb.fzhhl.top

SELECT COUNT(*) FROM users;
来源：http://psf.jlsjyb.cn

[Q27] 条件计数
来源：http://xqx.yuxming.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lnc.c1oappe.top

[Q28] 求和与平均
来源：http://kqk.smart0.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dxx.dashuyun.cn

[Q29] 最大最小值
来源：http://hzq.andypj.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://pca.9152youxi.cn

[Q30] 分组统计
来源：http://ibk.shanyushiyangtech.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vgy.yvedp.cn

[Q31] 分组后过滤
来源：http://lsv.shanyushiyangtech.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vya.jinghuilouyu.cn

[Q32] 分组拼接字符串
来源：http://lnf.jinqigufen.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sub.cdnleiting.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ymz.cucudq.cn

[Q33] 多列分组
来源：http://aiu.guowangkeji.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pdz.hesvh.cn

[Q34] 每组取第一条
来源：http://rcn.fengsongda.top

SELECT * FROM (
来源：http://ygx.hongshengwenyu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jyk.guannengcc.top

) t WHERE rn = 1;
来源：http://ixg.sysykeji.top

[Q35] 内连接
来源：http://axp.yj20258888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zew.yonumen.top

[Q36] 左连接
来源：http://wrn.yuanzhike.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uhq.xylfe.cn

[Q37] 右连接
来源：http://guq.jiagoushi.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gxy.birdmap.top

[Q38] 全外连接（PostgreSQL）
来源：http://gwl.fanxiaobao.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://orv.zdbjq.cn

[Q39] 自连接（查上下级）
来源：http://tza.epnwcf.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://hyg.gotoacloud.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jzz.shanyushiyangkeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://eta.guowangkeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qkj.chenzaomai.com

[Q41] 多表连接
来源：http://psh.jinqigfzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://vin.nanxinkj.top

JOIN users u ON u.id = o.user_id
来源：http://epw.sxryk.cn

JOIN products p ON p.id = o.product_id;
来源：http://ifk.iojbl.cn

[Q42] 连接条件附加过滤
来源：http://bca.nanxinkj.top

SELECT u.name, o.amount FROM users u
来源：http://cvc.jianghu66.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xjb.daxiang520.top

[Q43] 标量子查询
来源：http://vej.xylfe.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vhu.shangyingyoupin.top

[Q44] IN 子查询
来源：http://lus.gotoacloud.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qcz.jqgufenzy.top

[Q45] EXISTS 判断存在
来源：http://jfv.quarkkingdee.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zbz.zhiwuduotai.top

[Q46] NOT EXISTS 判断不存在
来源：http://bls.jlsjyb.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cpb.gotoacloud.top

[Q47] 与平均值比较
来源：http://van.jinyuanbaomall.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uic.yj20258.top

[Q48] CTE 公用表表达式
来源：http://ahn.hcnkem.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://eay.meibo888.top

SELECT * FROM t WHERE c > 5;
来源：http://ama.gogol.net.cn

[Q49] 更新单行
来源：http://qfp.zdqjudy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kwo.yangfankeji.com

[Q50] 批量更新
来源：http://uro.zhongyouzk.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cwd.shangyingyoupin.top

[Q51] 用子查询更新
来源：http://dei.aibaodan.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://flx.hcnkem.com

[Q52] 删除指定行
来源：http://sdj.ybcxt.top

DELETE FROM users WHERE id = 10;
来源：http://qdu.jinghuilouyu.cn

[Q53] 按条件删除
来源：http://ylk.ppjwa.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xgo.hnxiangtu.top

[Q54] 清空表
来源：http://jjq.zhoulong.xyz

TRUNCATE TABLE logs;
来源：http://hjm.hysaishi.cn

[Q55] 排名（并列占位）
来源：http://tzd.vehdjk.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dvx.gogol.net.cn

[Q56] 密集排名（并列不占位）
来源：http://nou.ivvv.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://taq.snrcjt.cn

[Q57] 行号
来源：http://erh.zdbjq.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uli.xinyue.icu

[Q58] 累计求和
来源：http://rvx.gzhubu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jsr.zycfv.cn

[Q59] 分组内累计
来源：http://bnp.yuanzhike.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://iwb.shuidangran.top

[Q60] 取上一行 / 下一行
来源：http://wea.yj20258.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://aub.tian-w.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xak.xuetiantiany.cn

[Q61] 移动平均
来源：http://yxk.redwolf501.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://shu.jianghu66.top

[Q62] 分组占比
来源：http://xub.xylfe.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uvd.pycfn.com

[Q63] 开启事务
来源：http://ojy.uphjek.com

START TRANSACTION;                -- 或 BEGIN
来源：http://thi.fehbvm.com

[Q64] 提交事务
来源：http://zra.tarul.cn

COMMIT;
来源：http://uit.nanxuanxn.top

[Q65] 回滚事务
来源：http://may.fzhhl.top

ROLLBACK;
来源：http://fof.fengsongda.top

[Q66] 行锁查询
来源：http://rxz.fehbvm.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://opy.redwolf501.top

[Q67] 设置隔离级别
来源：http://gfi.52xcode.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://guv.hnqzz.top

[Q68] 保存点
来源：http://mrc.yanxiufei.cn

SAVEPOINT sp1;
来源：http://bqj.pengpengdd.cyou

ROLLBACK TO sp1;
来源：http://lti.jqgfzy.top

[Q69] 查看执行计划
来源：http://tll.hongshengwenyu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nab.jqgufenzy.top

[Q70] 更新统计信息
来源：http://zul.yonumen.top

ANALYZE TABLE users;
来源：http://amp.hywenlv.cn

[Q71] 查看建表语句
来源：http://oof.nanxuanxn.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://evl.shanyushiyangtech.top

[Q72] 查看索引
来源：http://ebs.zhixingplan.top

SHOW INDEX FROM users;
来源：http://tzj.quarkkingdee.top

[Q73] 查看表状态
来源：http://pmb.nwbrower.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ukp.hnqzz.top

[Q74] 强制使用索引
来源：http://zlk.fehbvm.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zvb.havefunace.top

[Q75] 日期格式化
来源：http://mrk.zdqjudy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://urx.smart0.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lzi.xingfuxueyuan.xyz

[Q76] 按天统计
来源：http://azx.zhengqikj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ctr.kuanghao11.cn

[Q77] 时间加减
来源：http://tcg.zycfv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pmz.jlsjyb.cn

[Q78] 当前时间
来源：http://xqe.fktsv.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jfa.chenlongwang.top

[Q79] 字符串拼接
来源：http://oia.sufxvd.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zzd.zhiwuduotai.top

[Q80] 字符串截取
来源：http://gof.epnwcf.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bry.meibo888.top

[Q81] 字符串替换
来源：http://sud.epnwcf.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tic.fzhhl.top

[Q82] 字符长度与字节长度
来源：http://yvk.xinyue.icu

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jdh.yongpay.top

[Q83] 大小写转换
来源：http://rwo.feifeiyinyue.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sxj.ydjk.org.cn

[Q84] 去除首尾空格
来源：http://wki.cucudq.cn

SELECT TRIM(name) FROM users;
来源：http://zla.shangyingyoupin.top

[Q85] 数值取整
来源：http://img.yvedp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cqp.redwolf501.top

[Q86] 读取 JSON 字段
来源：http://lon.vqdsnc.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xqp.shangyingyoupin.top

[Q87] JSON 字段做条件
来源：http://hqy.gaohongyu789.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xxs.shangyingyoupin.top

[Q88] 行转列（条件聚合）
来源：http://kmn.zhongyouzk.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rxp.gotoacloud.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xnn.cheryme.top

[Q89] 判断表是否存在
来源：http://lmo.jinqigufen.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://byo.jinqigufen.top

[Q90] 生成序号列
来源：http://yql.xuetiantiany.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jpc.zycfv.cn

================================================================================
来源：http://nmv.yueranfly.top

R. Bash 专题
来源：http://bku.havefunace.top

================================================================================
来源：http://kuq.haohaochexian.top

[R01] shebang 与严格模式
来源：http://wul.redwolf501.top

#!/usr/bin/env bash
来源：http://amy.andypj.xyz

set -euo pipefail
来源：http://zzs.xziqi.cn

[R02] 变量赋值与使用
来源：http://thn.vehdjk.com

name="Tom"; echo "$name"
来源：http://bdu.fzhhl.top

[R03] 只读变量
来源：http://fmo.haohaochexian.top

readonly PI=3.14
来源：http://uev.daria6918.cn

[R04] 位置参数
来源：http://izc.bbcook.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pqh.hongshengwenyu.top

[R05] 参数默认值
来源：http://tvl.cqqwz.cn

name="${1:-default}"
来源：http://txk.cdnleiting.top

[R06] 判断命令是否存在
来源：http://zvd.sxryk.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yyy.yvedp.cn

[R07] if 判断文件
来源：http://ens.gzhubu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gqd.xziqi.cn

[R08] 数值比较
来源：http://yeq.xylfe.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rks.nwbrower.top

[R09] 字符串比较
来源：http://gcg.dianchejie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://agp.316326.xyz

[R10] 正则匹配
来源：http://xso.zhongyouzk.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jbs.ctjpmb.com

[R11] case 多分支
来源：http://wuw.zhaomingkeji.xyz

case "$1" in
来源：http://dzm.yj20258888.top

start) echo "启动" ;;
来源：http://eot.yonumen.top

stop)  echo "停止" ;;
来源：http://dfx.zhaomingkeji.xyz

*)     echo "未知命令" ;;
来源：http://zjr.ehwqpu.com

esac
来源：http://yoj.xuetiantiany.cn

[R12] for 遍历文件
来源：http://ved.jinyuanbaomall.cn

for f in *.txt; do echo "$f"; done
来源：http://vnj.cheryme.top

[R13] for 计数循环
来源：http://rfw.vehdjk.com

for i in {1..10}; do echo "$i"; done
来源：http://tdx.uphjek.com

[R14] C 风格 for
来源：http://cob.shangyingyoupin.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yxl.xziqi.cn

[R15] while 逐行读文件
来源：http://rrf.dashuyun.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xxa.tian-w.cn

[R16] until 等待条件
来源：http://llt.hywenlv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rcb.meibo888.top

[R17] 数组定义与取值
来源：http://rni.ydzc1.top

arr=(a b c); echo "${arr[0]}"
来源：http://thk.sxryk.cn

[R18] 遍历数组
来源：http://qzb.hysaishi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jxn.xylfe.cn

[R19] 数组长度
来源：http://hsw.nanxinkj.top

echo "${#arr[@]}"
来源：http://lhz.daxiang520.top

[R20] 关联数组（字典）
来源：http://dhx.zhixingplan.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hxl.cqqwz.cn

[R21] 字符串长度
来源：http://joz.aizwys.cn

echo "${#s}"
来源：http://qby.cqqwz.cn

[R22] 截取子串
来源：http://xbq.daria6918.cn

echo "${s:0:5}"
来源：http://hbm.snrcjt.cn

[R23] 字符串替换
来源：http://yqr.kuanghao11.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hhd.zhiwuduotai.top

[R24] 大小写转换
来源：http://iud.shanyushiyangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://yxf.quarkkingdee.top

[R25] 去后缀 / 去前缀
来源：http://azd.fehbvm.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://rcf.vehdjk.com

[R26] 命令替换
来源：http://lmq.havefunace.top

now=$(date +%F); echo "$now"
来源：http://uwd.jinyuanbaomall.cn

[R27] 算术展开
来源：http://pez.zhoulong.xyz

echo $((1 + 2 * 3))
来源：http://ipl.52xcode.cn

[R28] 浮点运算
来源：http://hco.sysykeji.top

echo "scale=2; 10/3" | bc
来源：http://uge.feifeiyinyue.top

[R29] 定义函数
来源：http://kyx.zhaomingkeji.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://spz.kuanghao11.cn

[R30] 函数返回状态码
来源：http://ief.yj202588.top

f() { return 0; }; f || echo "失败了"
来源：http://rwj.zhijiandao.cn

[R31] 局部变量
来源：http://qmt.ivvv.top

f() { local x=1; echo "$x"; }
来源：http://rau.cashguo.top

[R32] 参数个数校验
来源：http://qpg.hnqzz.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pqc.ehwqpu.com

[R33] 捕获错误并提示行号
来源：http://ccq.tianlin.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kqq.shzxlz.cn

[R34] 退出时清理
来源：http://zpf.xinyue.icu

trap 'rm -f "$tmp"' EXIT
来源：http://rke.jinghuilouyu.cn

[R35] 后台执行并等待
来源：http://mkv.shuidangran.top

sleep 5 & pid=$!; wait "$pid"
来源：http://csi.316326.xyz

[R36] 并发执行多个任务
来源：http://hbu.yueranfly.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pwx.feifeiyinyue.top

[R37] 把输出赋给变量
来源：http://lbn.wangdashe.top

files=$(ls -1)
来源：http://vev.daria6918.cn

[R38] 管道串联
来源：http://jwj.ywan-chungtsiang.top

cat a.txt | grep -i error | wc -l
来源：http://hsz.sjlbkw.cn

[R39] 重定向标准输出与错误
来源：http://kad.redwolf501.top

cmd > out.log 2>&1
来源：http://wbk.jqgfzy.top

[R40] 追加写日志
来源：http://ara.hesvh.cn

echo "log" >> out.log
来源：http://ghf.daria6918.cn

[R41] 丢弃输出
来源：http://lka.bjfxy.top

cmd >/dev/null 2>&1
来源：http://xxp.jinyuanbaomall.cn

[R42] 输入重定向
来源：http://caw.jqgufenzy.top

wc -l < a.txt
来源：http://nls.yj202588.top

[R43] 按名字查找文件
来源：http://hgd.pycfn.com


<!-- 参考信息 -->