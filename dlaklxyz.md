代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mfd.shangyingyoupin.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fwe.pycfn.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qig.jinyuanbaomall.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://frz.yanxiufei.cn

================================================================================
来源：http://gti.hongshengwenyu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wnv.yvedp.cn

================================================================================
来源：http://ldb.gaohongyu789.top

[Q01] 创建表
来源：http://duc.zdbjq.cn

CREATE TABLE users (
来源：http://zjs.nanxuanxn.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bbg.shuidangran.top

name VARCHAR(50) NOT NULL,
来源：http://wfm.tianlin.xyz

email VARCHAR(100) UNIQUE,
来源：http://mit.xuetiantiany.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hkz.hnxiangtu.top

);
来源：http://yni.meibo888.top

[Q02] 创建带外键的表
来源：http://mfn.zhengqikj.top

CREATE TABLE orders (
来源：http://pbu.shzxlz.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jng.havefunace.top

user_id INT NOT NULL,
来源：http://gcu.chenzaomai.com

amount DECIMAL(10, 2),
来源：http://ztk.xziqi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hal.yuxming.cn

);
来源：http://cch.iojbl.cn

[Q03] 增加列
来源：http://jdh.snrcjt.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://eoh.feifeiyinyue.top

[Q04] 修改列类型
来源：http://cti.sufxvd.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jay.yanxiufei.cn

[Q05] 重命名列
来源：http://plq.aibaodan.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hcr.yanxiufei.cn

[Q06] 删除列
来源：http://ypx.cashguo.top

ALTER TABLE users DROP COLUMN age;
来源：http://tgc.guannengcc.top

[Q07] 删除表
来源：http://tef.yvedp.cn

DROP TABLE IF EXISTS orders;
来源：http://vii.wangshuangyany.cn

[Q08] 创建普通索引
来源：http://pfb.nanxinkj.top

CREATE INDEX idx_users_email ON users(email);
来源：http://fmd.jinqigufen.top

[Q09] 创建唯一索引
来源：http://ibh.tian-w.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ije.zhoulong.xyz

[Q10] 插入单行
来源：http://ujb.xinyue.icu

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rao.zdbjq.cn

[Q11] 一次插入多行
来源：http://wck.hammf.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xht.kuanghao11.cn

[Q12] 插入后取自增 ID
来源：http://cov.aibaodan.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rhq.guowangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ljt.jinqigufen.top

[Q13] 忽略重复插入
来源：http://pbw.zhijiandao.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cnp.yonumen.top

[Q14] 存在则更新（upsert）
来源：http://kjg.kuanghao11.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://reo.dashuyun.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ced.xuanzx.com

[Q15] 查询全部
来源：http://ecc.sufxvd.cn

SELECT * FROM users;
来源：http://alp.zhiwuduotai.top

[Q16] 查询指定列
来源：http://lcy.ppjwa.cn

SELECT id, name FROM users;
来源：http://gdt.cheryme.top

[Q17] 条件查询
来源：http://izo.gaohongyu789.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://var.jyoumei.cn

[Q18] 模糊匹配
来源：http://lxa.svipenyu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jow.pycfn.com

[Q19] 范围查询
来源：http://jfp.xuetiantiany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tql.aizwys.cn

[Q20] IN 列表
来源：http://vme.hcnkem.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://aox.iojbl.cn

[Q21] 空值判断
来源：http://rqk.havefunace.top

SELECT * FROM users WHERE email IS NULL;
来源：http://vec.havefunace.top

[Q22] 排序
来源：http://sqo.daria6918.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wcm.9152youxi.cn

[Q23] 分页
来源：http://aej.ctjpmb.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rrh.jinqigfzy.top

[Q24] 去重
来源：http://bsb.tarul.cn

SELECT DISTINCT city FROM users;
来源：http://csl.jlsjyb.cn

[Q25] 只取前 N 条
来源：http://qck.hcnkem.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://txw.ehwqpu.com

[Q26] 计数
来源：http://eph.zhaomingkeji.xyz

SELECT COUNT(*) FROM users;
来源：http://sxi.fanxiaobao.xyz

[Q27] 条件计数
来源：http://wkx.0kj1m.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gvh.hysaishi.cn

[Q28] 求和与平均
来源：http://kij.wangshuangyany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vck.meibo888.top

[Q29] 最大最小值
来源：http://yux.cheryme.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://iim.nwbrower.top

[Q30] 分组统计
来源：http://nag.shanyushiyangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dwx.snrcjt.cn

[Q31] 分组后过滤
来源：http://qnw.shanyushiyangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ubt.cqqwz.cn

[Q32] 分组拼接字符串
来源：http://wye.yangfankeji.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ksx.jianghu66.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://utl.yangfankeji.com

[Q33] 多列分组
来源：http://lsi.epnwcf.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jfb.chenlongwang.top

[Q34] 每组取第一条
来源：http://izk.hnqzz.top

SELECT * FROM (
来源：http://bum.ydjk.org.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://iwl.yj20258.top

) t WHERE rn = 1;
来源：http://tkn.shanyushiyangtech.top

[Q35] 内连接
来源：http://eeh.jinyuanbaomall.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dvy.jqgufenzy.top

[Q36] 左连接
来源：http://qcv.shzxlz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hap.yj20258888.top

[Q37] 右连接
来源：http://ppo.shanyushiyangkeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://oeh.daxiang520.top

[Q38] 全外连接（PostgreSQL）
来源：http://mbp.pengpengdd.cyou

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mjz.tarul.cn

[Q39] 自连接（查上下级）
来源：http://agi.hysaishi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://csc.hysaishi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://put.gzhubu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://yuy.ybcxt.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rtv.hnqzz.top

[Q41] 多表连接
来源：http://njt.hongshengwenyu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rap.vehdjk.com

JOIN users u ON u.id = o.user_id
来源：http://ryc.iojbl.cn

JOIN products p ON p.id = o.product_id;
来源：http://fcy.9152youxi.cn

[Q42] 连接条件附加过滤
来源：http://ovv.hysaishi.cn

SELECT u.name, o.amount FROM users u
来源：http://yal.guannengcc.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ayp.nwbrower.top

[Q43] 标量子查询
来源：http://cai.cucudq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xiq.shuidangran.top

[Q44] IN 子查询
来源：http://flw.ivvv.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xsh.jinqigfzy.top

[Q45] EXISTS 判断存在
来源：http://kri.hcnkem.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dnj.yfazqb.com

[Q46] NOT EXISTS 判断不存在
来源：http://jav.fengsongda.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xdo.ehwqpu.com

[Q47] 与平均值比较
来源：http://uuv.dashuyun.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hoh.zhaomingkeji.xyz

[Q48] CTE 公用表表达式
来源：http://pkz.jinqigfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://som.feifeiyinyue.top

SELECT * FROM t WHERE c > 5;
来源：http://njj.jinqigfzy.top

[Q49] 更新单行
来源：http://luc.c1oappe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bgn.zhijiandao.cn

[Q50] 批量更新
来源：http://rux.uphjek.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hvh.daria6918.cn

[Q51] 用子查询更新
来源：http://vja.quarkkingdee.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wut.xingfuxueyuan.xyz

[Q52] 删除指定行
来源：http://whv.snrcjt.cn

DELETE FROM users WHERE id = 10;
来源：http://fus.dianchejie.cn

[Q53] 按条件删除
来源：http://bgw.zhaomingkeji.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tax.ydjk.org.cn

[Q54] 清空表
来源：http://nai.yuxming.cn

TRUNCATE TABLE logs;
来源：http://boj.jinghuilouyu.cn

[Q55] 排名（并列占位）
来源：http://dvy.tanke756.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tod.gotoacloud.top

[Q56] 密集排名（并列不占位）
来源：http://rse.vehdjk.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zza.guowangkeji.top

[Q57] 行号
来源：http://uwp.zhongyouzk.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bsu.cucudq.cn

[Q58] 累计求和
来源：http://lnx.bjfxy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://awe.fanxiaobao.xyz

[Q59] 分组内累计
来源：http://knu.0kj1m.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ixy.pycfn.com

[Q60] 取上一行 / 下一行
来源：http://grf.hammf.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://icm.svipenyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tvs.zhiwuduotai.top

[Q61] 移动平均
来源：http://edb.ivvv.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fjv.yonumen.top

[Q62] 分组占比
来源：http://ttb.jinyuanbaomall.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vus.pycfn.com

[Q63] 开启事务
来源：http://bjc.chenzaomai.com

START TRANSACTION;                -- 或 BEGIN
来源：http://rjy.tanke756.top

[Q64] 提交事务
来源：http://bpp.gotoacloud.top

COMMIT;
来源：http://ewb.xuetiantiany.cn

[Q65] 回滚事务
来源：http://rjo.zdbjq.cn

ROLLBACK;
来源：http://xoy.yangfankeji.com

[Q66] 行锁查询
来源：http://nes.jqgufenzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ejm.epnwcf.com

[Q67] 设置隔离级别
来源：http://kmx.shuidangran.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mjt.yonumen.top

[Q68] 保存点
来源：http://cti.havefunace.top

SAVEPOINT sp1;
来源：http://jhu.fanxiaobao.xyz

ROLLBACK TO sp1;
来源：http://dta.yuanzhike.top

[Q69] 查看执行计划
来源：http://ykt.zdbjq.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fer.guowangkeji.top

[Q70] 更新统计信息
来源：http://rdq.daxiang520.top

ANALYZE TABLE users;
来源：http://wpj.chenlongwang.top

[Q71] 查看建表语句
来源：http://acm.nanxinkj.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://deg.shanyushiyangtech.top

[Q72] 查看索引
来源：http://jbz.yueranfly.top

SHOW INDEX FROM users;
来源：http://izt.zhaomingkeji.xyz

[Q73] 查看表状态
来源：http://xjn.zycfv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xge.quarkkingdee.top

[Q74] 强制使用索引
来源：http://zuk.hesvh.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ugd.zhengqikj.top

[Q75] 日期格式化
来源：http://fcc.xingfuxueyuan.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ddp.wangshuangyany.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dkp.mhx1999.top

[Q76] 按天统计
来源：http://arn.svipenyu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qht.nwbrower.top

[Q77] 时间加减
来源：http://jkz.jinyuanbaomall.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vkf.yongpay.top

[Q78] 当前时间
来源：http://hzj.cucudq.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qkw.hnxiangtu.top

[Q79] 字符串拼接
来源：http://jpw.hnxiangtu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iav.yonumen.top

[Q80] 字符串截取
来源：http://ndd.zhixingplan.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jlx.52xcode.cn

[Q81] 字符串替换
来源：http://scv.daria6918.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://csj.cheryme.top

[Q82] 字符长度与字节长度
来源：http://jbv.cqqwz.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://win.jianghu66.top

[Q83] 大小写转换
来源：http://dio.daria6918.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://onw.pycfn.com

[Q84] 去除首尾空格
来源：http://oeb.hnxiangtu.top

SELECT TRIM(name) FROM users;
来源：http://cjo.havefunace.top

[Q85] 数值取整
来源：http://cfi.hfpthk.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://unb.sysykeji.top

[Q86] 读取 JSON 字段
来源：http://fln.daria6918.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xwl.nanxuanxn.top

[Q87] JSON 字段做条件
来源：http://kkn.guowangkeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hdc.yangfankeji.com

[Q88] 行转列（条件聚合）
来源：http://wlp.jqgufenzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lck.dashuyun.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://whi.cdnleiting.top

[Q89] 判断表是否存在
来源：http://bph.hnqzz.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wex.epnwcf.com

[Q90] 生成序号列
来源：http://pja.hcnkem.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://euq.yongpay.top

================================================================================
来源：http://ynl.tanke756.top

R. Bash 专题
来源：http://axx.xuanzx.com

================================================================================
来源：http://ljf.xingfuxueyuan.xyz

[R01] shebang 与严格模式
来源：http://zld.pengpengdd.cyou

#!/usr/bin/env bash
来源：http://lbe.jqgufenzy.top

set -euo pipefail
来源：http://ivk.yuanzhike.top

[R02] 变量赋值与使用
来源：http://gdj.wangdashe.top

name="Tom"; echo "$name"
来源：http://ewq.guannengcc.top

[R03] 只读变量
来源：http://anc.jinqigfzy.top

readonly PI=3.14
来源：http://izt.jiagoushi.top

[R04] 位置参数
来源：http://fee.gzhubu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hgq.sysykeji.top

[R05] 参数默认值
来源：http://imj.jianghu66.top

name="${1:-default}"
来源：http://zqa.nwbrower.top

[R06] 判断命令是否存在
来源：http://bvx.nanxuanxn.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kdw.dashuyun.cn

[R07] if 判断文件
来源：http://kuw.sysykeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nsw.fanxiaobao.xyz

[R08] 数值比较
来源：http://svc.jinghuilouyu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://iub.mhx1999.top

[R09] 字符串比较
来源：http://ljd.ctjpmb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fgg.dianchejie.cn

[R10] 正则匹配
来源：http://fgq.52xcode.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bao.tarul.cn

[R11] case 多分支
来源：http://vtp.9152youxi.cn

case "$1" in
来源：http://dia.zhongyouzk.top

start) echo "启动" ;;
来源：http://axg.guannengcc.top

stop)  echo "停止" ;;
来源：http://uqk.jqgufenzy.top

*)     echo "未知命令" ;;
来源：http://uui.jlsjyb.cn

esac
来源：http://qjd.c1oappe.top

[R12] for 遍历文件
来源：http://ocb.mhx1999.top

for f in *.txt; do echo "$f"; done
来源：http://fgs.yangfankeji.com

[R13] for 计数循环
来源：http://qtb.yueranfly.top

for i in {1..10}; do echo "$i"; done
来源：http://tzb.zhaomingkeji.xyz

[R14] C 风格 for
来源：http://nhs.fehbvm.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fqf.ybcxt.top

[R15] while 逐行读文件
来源：http://gza.ctjpmb.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ovm.zdbjq.cn

[R16] until 等待条件
来源：http://zia.zdqjudy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zxj.c1oappe.top

[R17] 数组定义与取值
来源：http://hbj.meibo888.top

arr=(a b c); echo "${arr[0]}"
来源：http://tmy.sweek.top

[R18] 遍历数组
来源：http://zni.tarul.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ajo.xingfuxueyuan.xyz

[R19] 数组长度
来源：http://kkq.cheryme.top

echo "${#arr[@]}"
来源：http://rkx.jqgufenzy.top

[R20] 关联数组（字典）
来源：http://std.ywan-chungtsiang.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zon.0kj1m.cn

[R21] 字符串长度
来源：http://fch.ppjwa.cn

echo "${#s}"
来源：http://dyp.yvedp.cn

[R22] 截取子串
来源：http://rjc.cucudq.cn

echo "${s:0:5}"
来源：http://vux.jianghu66.top

[R23] 字符串替换
来源：http://qdm.ywan-chungtsiang.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lnf.guannengcc.top

[R24] 大小写转换
来源：http://ify.fengsongda.top

echo "${s^^}"; echo "${s,,}"
来源：http://blo.hfpthk.cn

[R25] 去后缀 / 去前缀
来源：http://mjx.hfpthk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gly.daria6918.cn

[R26] 命令替换
来源：http://arc.yuanzhike.top

now=$(date +%F); echo "$now"
来源：http://dvn.yfazqb.com

[R27] 算术展开
来源：http://htu.hesvh.cn

echo $((1 + 2 * 3))
来源：http://sac.sufxvd.cn

[R28] 浮点运算
来源：http://azu.yonumen.top

echo "scale=2; 10/3" | bc
来源：http://glt.quarkkingdee.top

[R29] 定义函数
来源：http://hdi.wangshuangyany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ajl.tarul.cn

[R30] 函数返回状态码
来源：http://hrw.andypj.xyz

f() { return 0; }; f || echo "失败了"
来源：http://xvr.xinyue.icu

[R31] 局部变量
来源：http://taj.gotoacloud.top

f() { local x=1; echo "$x"; }
来源：http://nxs.fanxiaobao.xyz

[R32] 参数个数校验
来源：http://xjp.ppjwa.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uut.cheryme.top

[R33] 捕获错误并提示行号
来源：http://rtm.ywan-chungtsiang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jlr.fehbvm.com

[R34] 退出时清理
来源：http://ecw.sysykeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://jnz.fktsv.cn

[R35] 后台执行并等待
来源：http://gwk.pycfn.com

sleep 5 & pid=$!; wait "$pid"
来源：http://xfj.sysykeji.top

[R36] 并发执行多个任务
来源：http://aup.dashuyun.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mzv.nanxinkj.top

[R37] 把输出赋给变量
来源：http://jwg.jqgfzy.top

files=$(ls -1)
来源：http://unp.jiagoushi.top

[R38] 管道串联
来源：http://rny.sxryk.cn

cat a.txt | grep -i error | wc -l
来源：http://uks.chenjidiqi.icu

[R39] 重定向标准输出与错误
来源：http://xea.svipenyu.cn

cmd > out.log 2>&1
来源：http://xsa.9152youxi.cn

[R40] 追加写日志
来源：http://ztb.9152youxi.cn

echo "log" >> out.log
来源：http://svj.yueranfly.top

[R41] 丢弃输出
来源：http://rmw.fktsv.cn


<!-- 参考信息 -->