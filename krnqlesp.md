代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zvh.yanxiufei.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pqr.pycfn.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bxw.havefunace.top

[P08] 处理浮点精度问题
来源：http://qje.tianlin.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rvv.jqgufenzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://frn.gotoacloud.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jvk.yueranfly.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hin.meibo888.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qsu.hnqzz.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wbz.chenlongwang.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xrc.guowangkeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cfc.zhixingplan.top

================================================================================
来源：http://grr.yj20258888.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vyl.havefunace.top

================================================================================
来源：http://lgj.jlsjyb.cn

[Q01] 创建表
来源：http://dnl.yuxming.cn

CREATE TABLE users (
来源：http://hca.jinqigufen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tvk.hesvh.cn

name VARCHAR(50) NOT NULL,
来源：http://fzy.yvedp.cn

email VARCHAR(100) UNIQUE,
来源：http://akd.tarul.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dsg.0kj1m.cn

);
来源：http://dvq.0kj1m.cn

[Q02] 创建带外键的表
来源：http://iuf.fzhhl.top

CREATE TABLE orders (
来源：http://gpw.fehbvm.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nlp.zycfv.cn

user_id INT NOT NULL,
来源：http://axv.redwolf501.top

amount DECIMAL(10, 2),
来源：http://vuq.jinghuilouyu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pfg.gotoacloud.top

);
来源：http://yct.nwbrower.top

[Q03] 增加列
来源：http://rkh.ybcxt.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wid.xylfe.cn

[Q04] 修改列类型
来源：http://mbl.sjlbkw.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mun.yangfankeji.com

[Q05] 重命名列
来源：http://cyo.jqgufenzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gnn.chenjidiqi.icu

[Q06] 删除列
来源：http://ccy.sjlbkw.cn

ALTER TABLE users DROP COLUMN age;
来源：http://uxs.pycfn.com

[Q07] 删除表
来源：http://isx.aibaodan.cn

DROP TABLE IF EXISTS orders;
来源：http://nwz.sxryk.cn

[Q08] 创建普通索引
来源：http://bnz.sjlbkw.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tpx.cucudq.cn

[Q09] 创建唯一索引
来源：http://kng.yanxiufei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pzz.xinyue.icu

[Q10] 插入单行
来源：http://qnb.epnwcf.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://upj.yonumen.top

[Q11] 一次插入多行
来源：http://kth.pengpengdd.cyou

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bkw.chenjidiqi.icu

[Q12] 插入后取自增 ID
来源：http://zkd.zdqjudy.top

INSERT INTO users (name) VALUES ('C');
来源：http://ukn.zhengqikj.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dpd.aizwys.cn

[Q13] 忽略重复插入
来源：http://djl.chenlongwang.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rxj.jqgufenzy.top

[Q14] 存在则更新（upsert）
来源：http://sxa.ybcxt.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xlb.chenzaomai.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ixy.ehwqpu.com

[Q15] 查询全部
来源：http://vbd.dianchejie.cn

SELECT * FROM users;
来源：http://ygn.chenlongwang.top

[Q16] 查询指定列
来源：http://cee.tian-w.cn

SELECT id, name FROM users;
来源：http://yfd.fehbvm.com

[Q17] 条件查询
来源：http://sqh.zdbjq.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://byl.yonumen.top

[Q18] 模糊匹配
来源：http://mma.c1oappe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ctk.daria6918.cn

[Q19] 范围查询
来源：http://hog.yuanzhike.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xau.wangshuangyany.cn

[Q20] IN 列表
来源：http://ijp.nwbrower.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vmj.shuidangran.top

[Q21] 空值判断
来源：http://chz.cdnleiting.top

SELECT * FROM users WHERE email IS NULL;
来源：http://fcn.yvedp.cn

[Q22] 排序
来源：http://kdz.zhijiandao.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vtp.cheryme.top

[Q23] 分页
来源：http://unc.chenjidiqi.icu

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pha.yuanzhike.top

[Q24] 去重
来源：http://qgb.bjfxy.top

SELECT DISTINCT city FROM users;
来源：http://dps.zdqjudy.top

[Q25] 只取前 N 条
来源：http://yxm.dashuyun.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rym.yueranfly.top

[Q26] 计数
来源：http://acn.daria6918.cn

SELECT COUNT(*) FROM users;
来源：http://glj.haohaochexian.top

[Q27] 条件计数
来源：http://etm.yfazqb.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jqe.cqqwz.cn

[Q28] 求和与平均
来源：http://yvk.yuxming.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kia.9152youxi.cn

[Q29] 最大最小值
来源：http://byl.redwolf501.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://lhk.iojbl.cn

[Q30] 分组统计
来源：http://kbf.c1oappe.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bkd.hammf.cn

[Q31] 分组后过滤
来源：http://eoh.cqqwz.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wak.havefunace.top

[Q32] 分组拼接字符串
来源：http://ivl.zdqjudy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://otg.yuxming.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mfr.jinyuanbaomall.cn

[Q33] 多列分组
来源：http://rmh.xingfuxueyuan.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ibo.yj20258888.top

[Q34] 每组取第一条
来源：http://hvp.yangfankeji.com

SELECT * FROM (
来源：http://ydd.yj20258888.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ymt.aizwys.cn

) t WHERE rn = 1;
来源：http://nik.zhengqikj.top

[Q35] 内连接
来源：http://dso.ybcxt.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://spb.fktsv.cn

[Q36] 左连接
来源：http://zyl.haohaochexian.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vpr.cucudq.cn

[Q37] 右连接
来源：http://woe.zdbjq.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ezz.shanyushiyangtech.top

[Q38] 全外连接（PostgreSQL）
来源：http://yyi.zhongyouzk.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ics.smart0.xyz

[Q39] 自连接（查上下级）
来源：http://gsv.yuanzhike.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://sac.jianghu66.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vcn.andypj.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://wjb.jinqigufen.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tkb.yj20258888.top

[Q41] 多表连接
来源：http://uwl.yj202588.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://gfi.xuetiantiany.cn

JOIN users u ON u.id = o.user_id
来源：http://jnu.sweek.top

JOIN products p ON p.id = o.product_id;
来源：http://yub.yangfankeji.com

[Q42] 连接条件附加过滤
来源：http://abx.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u
来源：http://xec.cqqwz.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mvu.jianghu66.top

[Q43] 标量子查询
来源：http://vdh.pycfn.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://klo.ivvv.top

[Q44] IN 子查询
来源：http://kmm.bjfxy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://usy.redwolf501.top

[Q45] EXISTS 判断存在
来源：http://gpk.zhiwuduotai.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ppv.shanyushiyangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://rrh.dashuyun.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uet.fktsv.cn

[Q47] 与平均值比较
来源：http://bml.yj202588.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fwb.ywan-chungtsiang.top

[Q48] CTE 公用表表达式
来源：http://mpm.fzhhl.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ejd.gzhubu.top

SELECT * FROM t WHERE c > 5;
来源：http://yco.meibo888.top

[Q49] 更新单行
来源：http://pih.smart0.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dhy.hnxiangtu.top

[Q50] 批量更新
来源：http://ioe.andypj.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ieq.316326.xyz

[Q51] 用子查询更新
来源：http://aos.yuxming.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hsb.jqgfzy.top

[Q52] 删除指定行
来源：http://uka.snrcjt.cn

DELETE FROM users WHERE id = 10;
来源：http://xyv.guowangkeji.top

[Q53] 按条件删除
来源：http://lkx.meibo888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ifz.tianlin.xyz

[Q54] 清空表
来源：http://yez.jyoumei.cn

TRUNCATE TABLE logs;
来源：http://fal.pycfn.com

[Q55] 排名（并列占位）
来源：http://rmi.tarul.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lkv.daxiang520.top

[Q56] 密集排名（并列不占位）
来源：http://usb.gzhubu.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://eqa.meibo888.top

[Q57] 行号
来源：http://agr.zhijiandao.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xin.chenzaomai.com

[Q58] 累计求和
来源：http://qwe.sysykeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zgw.havefunace.top

[Q59] 分组内累计
来源：http://ljj.hcnkem.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hfn.zhijiandao.cn

[Q60] 取上一行 / 下一行
来源：http://zdw.jinqigfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://viv.fengsongda.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gwc.jqgfzy.top

[Q61] 移动平均
来源：http://hag.daxiang520.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oej.jinqigufen.top

[Q62] 分组占比
来源：http://dly.jinqigufen.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dut.bbcook.cn

[Q63] 开启事务
来源：http://qhb.yj202588.top

START TRANSACTION;                -- 或 BEGIN
来源：http://xgh.gzhubu.top

[Q64] 提交事务
来源：http://lwb.kuanghao11.cn

COMMIT;
来源：http://duw.shanyushiyangkeji.top

[Q65] 回滚事务
来源：http://fms.cheryme.top

ROLLBACK;
来源：http://mwq.zdqjudy.top

[Q66] 行锁查询
来源：http://wcm.sysykeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mme.vqdsnc.cn

[Q67] 设置隔离级别
来源：http://npb.daria6918.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rib.nanxuanxn.top

[Q68] 保存点
来源：http://crw.9152youxi.cn

SAVEPOINT sp1;
来源：http://fjq.daria6918.cn

ROLLBACK TO sp1;
来源：http://kjf.zhiwuduotai.top

[Q69] 查看执行计划
来源：http://cde.zdqjudy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fki.bjfxy.top

[Q70] 更新统计信息
来源：http://cjt.zdqjudy.top

ANALYZE TABLE users;
来源：http://zdl.9152youxi.cn

[Q71] 查看建表语句
来源：http://oum.yj20258.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xhb.quarkkingdee.top

[Q72] 查看索引
来源：http://zbz.hywenlv.cn

SHOW INDEX FROM users;
来源：http://dyz.hcnkem.com

[Q73] 查看表状态
来源：http://eos.hysaishi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wws.hfpthk.cn

[Q74] 强制使用索引
来源：http://xjh.daria6918.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mxi.tarul.cn

[Q75] 日期格式化
来源：http://flh.cashguo.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vby.dashuyun.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tnf.hongshengwenyu.top

[Q76] 按天统计
来源：http://bxr.dianchejie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://btc.yongpay.top

[Q77] 时间加减
来源：http://hks.meibo888.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tom.chenjidiqi.icu

[Q78] 当前时间
来源：http://wem.yj20258.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zgy.vehdjk.com

[Q79] 字符串拼接
来源：http://noc.zhaomingkeji.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://def.bjfxy.top

[Q80] 字符串截取
来源：http://gbp.jinqigufen.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xpb.wangshuangyany.cn

[Q81] 字符串替换
来源：http://vdy.cashguo.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hrc.quarkkingdee.top

[Q82] 字符长度与字节长度
来源：http://egg.shanyushiyangkeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zvt.9152youxi.cn

[Q83] 大小写转换
来源：http://rel.hywenlv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://llg.yj20258.top

[Q84] 去除首尾空格
来源：http://luu.zhiwuduotai.top

SELECT TRIM(name) FROM users;
来源：http://fng.52xcode.cn

[Q85] 数值取整
来源：http://vaz.nanxinkj.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mvq.jqgfzy.top

[Q86] 读取 JSON 字段
来源：http://zsv.cqqwz.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uds.pengpengdd.cyou

[Q87] JSON 字段做条件
来源：http://ikq.chenlongwang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hml.kuanghao11.cn

[Q88] 行转列（条件聚合）
来源：http://ola.ydzc1.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mru.jyoumei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jzs.jqgufenzy.top

[Q89] 判断表是否存在
来源：http://dge.kuanghao11.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zdo.snrcjt.cn

[Q90] 生成序号列
来源：http://qxu.jinqigfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ynk.yuanzhike.top

================================================================================
来源：http://ydn.ywan-chungtsiang.top

R. Bash 专题
来源：http://wwr.iojbl.cn

================================================================================
来源：http://liy.hammf.cn

[R01] shebang 与严格模式
来源：http://lai.shangyingyoupin.top

#!/usr/bin/env bash
来源：http://ccu.fehbvm.com

set -euo pipefail
来源：http://myb.yangfankeji.com

[R02] 变量赋值与使用
来源：http://aqo.hcnkem.com

name="Tom"; echo "$name"
来源：http://oey.jqgufenzy.top

[R03] 只读变量
来源：http://nkm.ydzc1.top

readonly PI=3.14
来源：http://osn.jinyuanbaomall.cn

[R04] 位置参数
来源：http://xra.cashguo.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fmx.ydjk.org.cn

[R05] 参数默认值
来源：http://gat.nwbrower.top

name="${1:-default}"
来源：http://ips.pycfn.com

[R06] 判断命令是否存在
来源：http://scj.yvedp.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://txo.jinqigfzy.top

[R07] if 判断文件
来源：http://pxf.zhiwuduotai.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hyk.gogol.net.cn

[R08] 数值比较
来源：http://olo.ywan-chungtsiang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://atv.yanxiufei.cn

[R09] 字符串比较
来源：http://wsi.feifeiyinyue.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fit.shanyushiyangkeji.top

[R10] 正则匹配
来源：http://nvx.yj202588.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wwt.wangdashe.top

[R11] case 多分支
来源：http://frs.tian-w.cn

case "$1" in
来源：http://fne.hcnkem.com

start) echo "启动" ;;
来源：http://ybt.snrcjt.cn

stop)  echo "停止" ;;
来源：http://izn.zhoulong.xyz

*)     echo "未知命令" ;;
来源：http://otp.xziqi.cn

esac
来源：http://tyu.nwbrower.top

[R12] for 遍历文件
来源：http://zyz.jiagoushi.top

for f in *.txt; do echo "$f"; done
来源：http://xhy.ctjpmb.com

[R13] for 计数循环
来源：http://cak.jinqigufen.top

for i in {1..10}; do echo "$i"; done
来源：http://vrb.xziqi.cn

[R14] C 风格 for
来源：http://vwl.kuanghao11.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://eld.hnqzz.top

[R15] while 逐行读文件
来源：http://yga.havefunace.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://onx.yanxiufei.cn

[R16] until 等待条件
来源：http://bcb.hesvh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zlx.xuanzx.com

[R17] 数组定义与取值
来源：http://kkc.ydzc1.top

arr=(a b c); echo "${arr[0]}"
来源：http://kxw.hysaishi.cn

[R18] 遍历数组
来源：http://dsk.fanxiaobao.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vit.chenlongwang.top

[R19] 数组长度
来源：http://nvn.daxiang520.top

echo "${#arr[@]}"
来源：http://prs.sysykeji.top

[R20] 关联数组（字典）
来源：http://gjw.hnxiangtu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kxq.jinqigufen.top

[R21] 字符串长度
来源：http://mxk.jiagoushi.top

echo "${#s}"
来源：http://xjv.cheryme.top

[R22] 截取子串
来源：http://med.yj202588.top

echo "${s:0:5}"
来源：http://uii.hnxiangtu.top

[R23] 字符串替换
来源：http://ryj.ydzc1.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wbb.zdqjudy.top

[R24] 大小写转换
来源：http://qbh.jinqigfzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://oac.quarkkingdee.top

[R25] 去后缀 / 去前缀
来源：http://ern.hfpthk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rwt.hongshengwenyu.top

[R26] 命令替换
来源：http://egd.guowangkeji.top

now=$(date +%F); echo "$now"
来源：http://awz.xinyue.icu

[R27] 算术展开
来源：http://wgj.bbcook.cn

echo $((1 + 2 * 3))
来源：http://ulq.ctjpmb.com

[R28] 浮点运算
来源：http://kik.hcnkem.com

echo "scale=2; 10/3" | bc
来源：http://dew.yonumen.top

[R29] 定义函数
来源：http://jgc.hcnkem.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yin.9152youxi.cn

[R30] 函数返回状态码
来源：http://nqr.hnqzz.top

f() { return 0; }; f || echo "失败了"
来源：http://uef.gaohongyu789.top

[R31] 局部变量
来源：http://qau.dianchejie.cn

f() { local x=1; echo "$x"; }
来源：http://mwe.yanxiufei.cn

[R32] 参数个数校验
来源：http://vfa.fengsongda.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oyr.jyoumei.cn

[R33] 捕获错误并提示行号
来源：http://sik.jinqigufen.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kzz.redwolf501.top

[R34] 退出时清理
来源：http://nyi.yuanzhike.top

trap 'rm -f "$tmp"' EXIT
来源：http://dbw.shangyingyoupin.top

[R35] 后台执行并等待
来源：http://nog.aizwys.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bit.xylfe.cn

[R36] 并发执行多个任务
来源：http://blu.bjfxy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mgd.hfpthk.cn

[R37] 把输出赋给变量
来源：http://nto.gotoacloud.top


<!-- 参考信息 -->