代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jxm.zhaomingkeji.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jvv.fzhhl.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xvj.gzhubu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dkd.tian-w.cn

================================================================================
来源：http://lfc.zhijiandao.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://odo.xinyue.icu

================================================================================
来源：http://xso.52xcode.cn

[Q01] 创建表
来源：http://rcj.zhijiandao.cn

CREATE TABLE users (
来源：http://ogt.chenzaomai.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xmd.ydzc1.top

name VARCHAR(50) NOT NULL,
来源：http://imt.hywenlv.cn

email VARCHAR(100) UNIQUE,
来源：http://adf.jiagoushi.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fnx.pengpengdd.cyou

);
来源：http://fjm.zhongyouzk.top

[Q02] 创建带外键的表
来源：http://qfw.chenlongwang.top

CREATE TABLE orders (
来源：http://wqc.sjlbkw.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ako.jinqigufen.top

user_id INT NOT NULL,
来源：http://anv.fengsongda.top

amount DECIMAL(10, 2),
来源：http://zeu.jianghu66.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tae.zdbjq.cn

);
来源：http://sax.zycfv.cn

[Q03] 增加列
来源：http://ikz.zdbjq.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kmf.ydjk.org.cn

[Q04] 修改列类型
来源：http://ulp.yueranfly.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jfl.pengpengdd.cyou

[Q05] 重命名列
来源：http://frc.svipenyu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vcw.316326.xyz

[Q06] 删除列
来源：http://sgc.ydzc1.top

ALTER TABLE users DROP COLUMN age;
来源：http://rzd.jqgufenzy.top

[Q07] 删除表
来源：http://sna.jqgfzy.top

DROP TABLE IF EXISTS orders;
来源：http://mgq.epnwcf.com

[Q08] 创建普通索引
来源：http://dum.vqdsnc.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ztx.yj20258.top

[Q09] 创建唯一索引
来源：http://dnr.bjfxy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bhq.sufxvd.cn

[Q10] 插入单行
来源：http://ixr.hongshengwenyu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jan.hywenlv.cn

[Q11] 一次插入多行
来源：http://rny.daria6918.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sgf.ctjpmb.com

[Q12] 插入后取自增 ID
来源：http://gzq.sjlbkw.cn

INSERT INTO users (name) VALUES ('C');
来源：http://txx.gzhubu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lni.xuanzx.com

[Q13] 忽略重复插入
来源：http://txw.xuanzx.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://guy.xuetiantiany.cn

[Q14] 存在则更新（upsert）
来源：http://wvl.uphjek.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wyh.sjlbkw.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gcm.0kj1m.cn

[Q15] 查询全部
来源：http://mbs.nanxuanxn.top

SELECT * FROM users;
来源：http://fnp.jianghu66.top

[Q16] 查询指定列
来源：http://dpg.shzxlz.cn

SELECT id, name FROM users;
来源：http://nzq.havefunace.top

[Q17] 条件查询
来源：http://owx.fanxiaobao.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://huv.shanyushiyangkeji.top

[Q18] 模糊匹配
来源：http://dha.zhoulong.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://esu.sxryk.cn

[Q19] 范围查询
来源：http://clg.fehbvm.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mga.c1oappe.top

[Q20] IN 列表
来源：http://nyl.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://esk.epnwcf.com

[Q21] 空值判断
来源：http://knd.gogol.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://omp.zhaomingkeji.xyz

[Q22] 排序
来源：http://wua.chenlongwang.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://byc.shangyingyoupin.top

[Q23] 分页
来源：http://yuc.daxiang520.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bxg.xingfuxueyuan.xyz

[Q24] 去重
来源：http://har.pengpengdd.cyou

SELECT DISTINCT city FROM users;
来源：http://sxr.sxryk.cn

[Q25] 只取前 N 条
来源：http://iqa.meibo888.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cqw.daxiang520.top

[Q26] 计数
来源：http://mgg.jinyuanbaomall.cn

SELECT COUNT(*) FROM users;
来源：http://hll.yanxiufei.cn

[Q27] 条件计数
来源：http://atn.sufxvd.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qqb.xuanzx.com

[Q28] 求和与平均
来源：http://lpl.tian-w.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xre.cheryme.top

[Q29] 最大最小值
来源：http://qvd.vqdsnc.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pxg.fengsongda.top

[Q30] 分组统计
来源：http://izg.yangfankeji.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dgq.daria6918.cn

[Q31] 分组后过滤
来源：http://fjq.mhx1999.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qpu.nanxinkj.top

[Q32] 分组拼接字符串
来源：http://xhz.chenlongwang.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hwi.xinyue.icu

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mxr.shanyushiyangkeji.top

[Q33] 多列分组
来源：http://azg.zhijiandao.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://axw.tanke756.top

[Q34] 每组取第一条
来源：http://rfe.birdmap.top

SELECT * FROM (
来源：http://tlv.birdmap.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mmc.tarul.cn

) t WHERE rn = 1;
来源：http://shl.fengsongda.top

[Q35] 内连接
来源：http://cag.haohaochexian.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://don.svipenyu.cn

[Q36] 左连接
来源：http://roj.cucudq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://csk.vehdjk.com

[Q37] 右连接
来源：http://sgi.ydzc1.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jzp.yuanzhike.top

[Q38] 全外连接（PostgreSQL）
来源：http://arf.daxiang520.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wer.fzhhl.top

[Q39] 自连接（查上下级）
来源：http://bgc.fanxiaobao.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://pmd.shangyingyoupin.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://njd.xziqi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vhi.fehbvm.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bas.jinghuilouyu.cn

[Q41] 多表连接
来源：http://cni.xuanzx.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://fwp.epnwcf.com

JOIN users u ON u.id = o.user_id
来源：http://ddm.hysaishi.cn

JOIN products p ON p.id = o.product_id;
来源：http://ezv.hnxiangtu.top

[Q42] 连接条件附加过滤
来源：http://dej.fehbvm.com

SELECT u.name, o.amount FROM users u
来源：http://eed.yj202588.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gyy.yfazqb.com

[Q43] 标量子查询
来源：http://chm.fanxiaobao.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://iti.52xcode.cn

[Q44] IN 子查询
来源：http://dsd.ppjwa.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uad.yuanzhike.top

[Q45] EXISTS 判断存在
来源：http://zul.ctjpmb.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ojq.aibaodan.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wmi.cucudq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ogw.yuanzhike.top

[Q47] 与平均值比较
来源：http://xom.sjlbkw.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://awj.shanyushiyangtech.top

[Q48] CTE 公用表表达式
来源：http://xaq.sjlbkw.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zqf.meibo888.top

SELECT * FROM t WHERE c > 5;
来源：http://bxk.guowangkeji.top

[Q49] 更新单行
来源：http://ibd.jinqigfzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bee.yangfankeji.com

[Q50] 批量更新
来源：http://ydu.andypj.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zwb.tarul.cn

[Q51] 用子查询更新
来源：http://sxc.xylfe.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nre.yuxming.cn

[Q52] 删除指定行
来源：http://vry.guowangkeji.top

DELETE FROM users WHERE id = 10;
来源：http://bpw.chenzaomai.com

[Q53] 按条件删除
来源：http://nii.aizwys.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mhp.aizwys.cn

[Q54] 清空表
来源：http://hlr.ydjk.org.cn

TRUNCATE TABLE logs;
来源：http://ynf.zhengqikj.top

[Q55] 排名（并列占位）
来源：http://axb.fanxiaobao.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fss.chenlongwang.top

[Q56] 密集排名（并列不占位）
来源：http://wpq.ppjwa.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pmv.yanxiufei.cn

[Q57] 行号
来源：http://xzx.tianlin.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hve.fanxiaobao.xyz

[Q58] 累计求和
来源：http://alb.cdnleiting.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qdq.c1oappe.top

[Q59] 分组内累计
来源：http://lkb.zhiwuduotai.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nrc.ehwqpu.com

[Q60] 取上一行 / 下一行
来源：http://emw.cashguo.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xcx.epnwcf.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://muj.shangyingyoupin.top

[Q61] 移动平均
来源：http://ncf.gaohongyu789.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uea.xingfuxueyuan.xyz

[Q62] 分组占比
来源：http://bfe.hnqzz.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nux.gaohongyu789.top

[Q63] 开启事务
来源：http://gjm.cheryme.top

START TRANSACTION;                -- 或 BEGIN
来源：http://soc.tianlin.xyz

[Q64] 提交事务
来源：http://bjs.aizwys.cn

COMMIT;
来源：http://vsi.jqgfzy.top

[Q65] 回滚事务
来源：http://rgf.jinyuanbaomall.cn

ROLLBACK;
来源：http://ywy.cucudq.cn

[Q66] 行锁查询
来源：http://sat.yongpay.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qet.fanxiaobao.xyz

[Q67] 设置隔离级别
来源：http://hvh.bbcook.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gua.zhengqikj.top

[Q68] 保存点
来源：http://ekm.yuxming.cn

SAVEPOINT sp1;
来源：http://vur.jinyuanbaomall.cn

ROLLBACK TO sp1;
来源：http://gnz.feifeiyinyue.top

[Q69] 查看执行计划
来源：http://cdw.ivvv.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vwz.vqdsnc.cn

[Q70] 更新统计信息
来源：http://bhp.yangfankeji.com

ANALYZE TABLE users;
来源：http://zcz.nanxuanxn.top

[Q71] 查看建表语句
来源：http://ndf.jinyuanbaomall.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rat.hnqzz.top

[Q72] 查看索引
来源：http://ixk.zhongyouzk.top

SHOW INDEX FROM users;
来源：http://cbc.pycfn.com

[Q73] 查看表状态
来源：http://oyb.52xcode.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://yxz.jinyuanbaomall.cn

[Q74] 强制使用索引
来源：http://fea.vqdsnc.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wxl.ppjwa.cn

[Q75] 日期格式化
来源：http://zrv.yangfankeji.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://obq.zdbjq.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://irp.hywenlv.cn

[Q76] 按天统计
来源：http://exl.jiagoushi.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oun.yuanzhike.top

[Q77] 时间加减
来源：http://ydc.dashuyun.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kaw.gotoacloud.top

[Q78] 当前时间
来源：http://rqw.zhoulong.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nxn.yonumen.top

[Q79] 字符串拼接
来源：http://vpv.jlsjyb.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rsx.gotoacloud.top

[Q80] 字符串截取
来源：http://rea.nanxinkj.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nga.zhiwuduotai.top

[Q81] 字符串替换
来源：http://xms.aibaodan.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sse.xinyue.icu

[Q82] 字符长度与字节长度
来源：http://rvt.hnxiangtu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uff.xylfe.cn

[Q83] 大小写转换
来源：http://dps.sweek.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ekl.zhengqikj.top

[Q84] 去除首尾空格
来源：http://hzm.jqgufenzy.top

SELECT TRIM(name) FROM users;
来源：http://zgu.andypj.xyz

[Q85] 数值取整
来源：http://tne.guannengcc.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://psh.jyoumei.cn

[Q86] 读取 JSON 字段
来源：http://afw.ehwqpu.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nmb.nanxinkj.top

[Q87] JSON 字段做条件
来源：http://hdm.feifeiyinyue.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://aet.chenlongwang.top

[Q88] 行转列（条件聚合）
来源：http://ybn.jinqigfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mfz.zhiwuduotai.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://idv.jlsjyb.cn

[Q89] 判断表是否存在
来源：http://zfv.jiagoushi.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tkj.yueranfly.top

[Q90] 生成序号列
来源：http://fks.smart0.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://czl.ppjwa.cn

================================================================================
来源：http://kja.jianghu66.top

R. Bash 专题
来源：http://zlh.yongpay.top

================================================================================
来源：http://khr.nwbrower.top

[R01] shebang 与严格模式
来源：http://ojb.yonumen.top

#!/usr/bin/env bash
来源：http://chn.sjlbkw.cn

set -euo pipefail
来源：http://jbx.xingfuxueyuan.xyz

[R02] 变量赋值与使用
来源：http://vrp.yj20258.top

name="Tom"; echo "$name"
来源：http://hmk.wangshuangyany.cn

[R03] 只读变量
来源：http://vws.xuanzx.com

readonly PI=3.14
来源：http://fou.tianlin.xyz

[R04] 位置参数
来源：http://inp.yuanzhike.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ovj.yangfankeji.com

[R05] 参数默认值
来源：http://oyv.sxryk.cn

name="${1:-default}"
来源：http://noc.ywan-chungtsiang.top

[R06] 判断命令是否存在
来源：http://wig.zhijiandao.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hky.316326.xyz

[R07] if 判断文件
来源：http://qyv.zhixingplan.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://egt.sjlbkw.cn

[R08] 数值比较
来源：http://uoy.jlsjyb.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://uex.fengsongda.top

[R09] 字符串比较
来源：http://gsa.zhaomingkeji.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zdp.havefunace.top

[R10] 正则匹配
来源：http://nsr.zhaomingkeji.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nbc.shanyushiyangkeji.top

[R11] case 多分支
来源：http://cyg.ctjpmb.com

case "$1" in
来源：http://sbd.nwbrower.top

start) echo "启动" ;;
来源：http://jer.ybcxt.top

stop)  echo "停止" ;;
来源：http://txe.jlsjyb.cn

*)     echo "未知命令" ;;
来源：http://czi.316326.xyz

esac
来源：http://unr.dashuyun.cn

[R12] for 遍历文件
来源：http://bil.yj20258888.top

for f in *.txt; do echo "$f"; done
来源：http://zuz.9152youxi.cn

[R13] for 计数循环
来源：http://icm.yfazqb.com

for i in {1..10}; do echo "$i"; done
来源：http://iti.xylfe.cn

[R14] C 风格 for
来源：http://vsq.hesvh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sbe.jinyuanbaomall.cn

[R15] while 逐行读文件
来源：http://ora.xuanzx.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yic.meibo888.top

[R16] until 等待条件
来源：http://zta.gogol.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://grg.fzhhl.top

[R17] 数组定义与取值
来源：http://crg.jiagoushi.top

arr=(a b c); echo "${arr[0]}"
来源：http://cax.birdmap.top

[R18] 遍历数组
来源：http://apb.shuidangran.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ohj.cheryme.top

[R19] 数组长度
来源：http://yjp.jianghu66.top

echo "${#arr[@]}"
来源：http://ymh.ivvv.top

[R20] 关联数组（字典）
来源：http://eli.pengpengdd.cyou

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ujf.hnqzz.top

[R21] 字符串长度
来源：http://bqx.shanyushiyangkeji.top

echo "${#s}"
来源：http://dft.hnxiangtu.top

[R22] 截取子串
来源：http://qkw.yonumen.top

echo "${s:0:5}"
来源：http://ola.feifeiyinyue.top

[R23] 字符串替换
来源：http://vvi.havefunace.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://his.svipenyu.cn

[R24] 大小写转换
来源：http://tdm.jqgufenzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://jjz.wangdashe.top

[R25] 去后缀 / 去前缀
来源：http://sdd.shanyushiyangkeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://mzm.tianlin.xyz

[R26] 命令替换
来源：http://sjv.svipenyu.cn

now=$(date +%F); echo "$now"
来源：http://onu.yj202588.top

[R27] 算术展开
来源：http://hrz.shanyushiyangtech.top

echo $((1 + 2 * 3))
来源：http://mgg.xingfuxueyuan.xyz

[R28] 浮点运算
来源：http://idt.shanyushiyangtech.top

echo "scale=2; 10/3" | bc
来源：http://sah.hammf.cn

[R29] 定义函数
来源：http://gul.zhijiandao.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lwj.0kj1m.cn

[R30] 函数返回状态码
来源：http://jqj.shzxlz.cn

f() { return 0; }; f || echo "失败了"
来源：http://nwl.52xcode.cn

[R31] 局部变量
来源：http://ryj.shangyingyoupin.top

f() { local x=1; echo "$x"; }
来源：http://dcc.sufxvd.cn

[R32] 参数个数校验
来源：http://qva.zhengqikj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ats.ctjpmb.com

[R33] 捕获错误并提示行号
来源：http://uao.cashguo.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://top.pycfn.com

[R34] 退出时清理
来源：http://vkf.52xcode.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mjz.tanke756.top

[R35] 后台执行并等待
来源：http://bsd.uphjek.com

sleep 5 & pid=$!; wait "$pid"
来源：http://wbj.hesvh.cn

[R36] 并发执行多个任务
来源：http://rdp.yonumen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sem.feifeiyinyue.top

[R37] 把输出赋给变量
来源：http://psi.wangdashe.top

files=$(ls -1)
来源：http://ehf.chenzaomai.com

[R38] 管道串联
来源：http://hmb.yj202588.top

cat a.txt | grep -i error | wc -l
来源：http://yog.yangfankeji.com

[R39] 重定向标准输出与错误
来源：http://fpw.zdqjudy.top

cmd > out.log 2>&1
来源：http://mzh.xziqi.cn

[R40] 追加写日志
来源：http://nhb.kuanghao11.cn

echo "log" >> out.log
来源：http://itr.hfpthk.cn

[R41] 丢弃输出
来源：http://prm.yueranfly.top


<!-- 参考信息 -->