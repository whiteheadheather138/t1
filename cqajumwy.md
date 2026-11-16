代发 wailian999

================================================================================
来源：http://nls.zhongyouzk.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uic.havefunace.top

================================================================================
来源：http://fiz.yuxming.cn

[Q01] 创建表
来源：http://pop.hcnkem.com

CREATE TABLE users (
来源：http://vcg.uphjek.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pxm.shuidangran.top

name VARCHAR(50) NOT NULL,
来源：http://zez.wangdashe.top

email VARCHAR(100) UNIQUE,
来源：http://bez.chenlongwang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gas.yonumen.top

);
来源：http://pdz.quarkkingdee.top

[Q02] 创建带外键的表
来源：http://ppk.ivvv.top

CREATE TABLE orders (
来源：http://kwl.ppjwa.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fis.pengpengdd.cyou

user_id INT NOT NULL,
来源：http://yjr.jinghuilouyu.cn

amount DECIMAL(10, 2),
来源：http://mgc.sufxvd.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dmy.yj20258888.top

);
来源：http://phu.yj20258.top

[Q03] 增加列
来源：http://byq.chenzaomai.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://agd.yueranfly.top

[Q04] 修改列类型
来源：http://lpt.zdqjudy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jou.nanxinkj.top

[Q05] 重命名列
来源：http://lbv.zycfv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bup.zhoulong.xyz

[Q06] 删除列
来源：http://jpa.jinqigfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://pil.feifeiyinyue.top

[Q07] 删除表
来源：http://bfi.jiagoushi.top

DROP TABLE IF EXISTS orders;
来源：http://vct.yfazqb.com

[Q08] 创建普通索引
来源：http://fre.52xcode.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zfg.yuanzhike.top

[Q09] 创建唯一索引
来源：http://prj.jinyuanbaomall.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://huy.haohaochexian.top

[Q10] 插入单行
来源：http://rnb.sjlbkw.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://otu.shanyushiyangtech.top

[Q11] 一次插入多行
来源：http://daa.ehwqpu.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ceu.zhaomingkeji.xyz

[Q12] 插入后取自增 ID
来源：http://dbk.daxiang520.top

INSERT INTO users (name) VALUES ('C');
来源：http://yqe.havefunace.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qjs.shzxlz.cn

[Q13] 忽略重复插入
来源：http://dll.xuetiantiany.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kmq.zhiwuduotai.top

[Q14] 存在则更新（upsert）
来源：http://xci.vqdsnc.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://add.tarul.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cuy.smart0.xyz

[Q15] 查询全部
来源：http://kcs.sufxvd.cn

SELECT * FROM users;
来源：http://uda.feifeiyinyue.top

[Q16] 查询指定列
来源：http://kry.xziqi.cn

SELECT id, name FROM users;
来源：http://mmy.zhixingplan.top

[Q17] 条件查询
来源：http://wvc.shzxlz.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kyh.aizwys.cn

[Q18] 模糊匹配
来源：http://swz.sufxvd.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vyx.gaohongyu789.top

[Q19] 范围查询
来源：http://gyw.xylfe.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dfs.yuanzhike.top

[Q20] IN 列表
来源：http://yww.redwolf501.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rds.tian-w.cn

[Q21] 空值判断
来源：http://cfp.nanxinkj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://kdt.316326.xyz

[Q22] 排序
来源：http://ujb.redwolf501.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uht.ctjpmb.com

[Q23] 分页
来源：http://vgf.hammf.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jrz.zdqjudy.top

[Q24] 去重
来源：http://hzp.pycfn.com

SELECT DISTINCT city FROM users;
来源：http://beq.fengsongda.top

[Q25] 只取前 N 条
来源：http://qkm.ybcxt.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://miq.ehwqpu.com

[Q26] 计数
来源：http://yln.hfpthk.cn

SELECT COUNT(*) FROM users;
来源：http://axy.sufxvd.cn

[Q27] 条件计数
来源：http://lhk.0kj1m.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ovq.jqgfzy.top

[Q28] 求和与平均
来源：http://tjk.jiagoushi.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dkh.hysaishi.cn

[Q29] 最大最小值
来源：http://ogh.sysykeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xic.fehbvm.com

[Q30] 分组统计
来源：http://cxf.jinghuilouyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xzt.jinyuanbaomall.cn

[Q31] 分组后过滤
来源：http://kfw.tanke756.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zyj.zhongyouzk.top

[Q32] 分组拼接字符串
来源：http://pfg.chenzaomai.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oez.zhijiandao.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xae.xylfe.cn

[Q33] 多列分组
来源：http://zpm.dashuyun.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wwa.yj20258888.top

[Q34] 每组取第一条
来源：http://waw.tianlin.xyz

SELECT * FROM (
来源：http://lfo.hnxiangtu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yxg.birdmap.top

) t WHERE rn = 1;
来源：http://dko.ehwqpu.com

[Q35] 内连接
来源：http://oqz.zdbjq.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nli.hesvh.cn

[Q36] 左连接
来源：http://xiw.zhongyouzk.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bav.wangdashe.top

[Q37] 右连接
来源：http://ehm.daria6918.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dhd.zhengqikj.top

[Q38] 全外连接（PostgreSQL）
来源：http://qae.jinqigfzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bxv.ivvv.top

[Q39] 自连接（查上下级）
来源：http://qsk.iojbl.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://uki.chenlongwang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dxe.jinyuanbaomall.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bhb.cqqwz.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ruq.uphjek.com

[Q41] 多表连接
来源：http://ndn.9152youxi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cqf.hfpthk.cn

JOIN users u ON u.id = o.user_id
来源：http://tut.epnwcf.com

JOIN products p ON p.id = o.product_id;
来源：http://bjk.sxryk.cn

[Q42] 连接条件附加过滤
来源：http://pbt.yuxming.cn

SELECT u.name, o.amount FROM users u
来源：http://uit.gzhubu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://myo.hnxiangtu.top

[Q43] 标量子查询
来源：http://ogr.jinghuilouyu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qlu.gzhubu.top

[Q44] IN 子查询
来源：http://xyn.epnwcf.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xya.iojbl.cn

[Q45] EXISTS 判断存在
来源：http://prr.chenzaomai.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tzp.yj20258888.top

[Q46] NOT EXISTS 判断不存在
来源：http://ysa.dianchejie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gha.kuanghao11.cn

[Q47] 与平均值比较
来源：http://spg.fengsongda.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uiw.smart0.xyz

[Q48] CTE 公用表表达式
来源：http://pur.cdnleiting.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ejn.hnqzz.top

SELECT * FROM t WHERE c > 5;
来源：http://pgy.ywan-chungtsiang.top

[Q49] 更新单行
来源：http://dxu.chenlongwang.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yvc.yvedp.cn

[Q50] 批量更新
来源：http://nvz.yueranfly.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hzg.zhoulong.xyz

[Q51] 用子查询更新
来源：http://lwy.yangfankeji.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hul.xingfuxueyuan.xyz

[Q52] 删除指定行
来源：http://lob.zhijiandao.cn

DELETE FROM users WHERE id = 10;
来源：http://ebh.zycfv.cn

[Q53] 按条件删除
来源：http://pui.redwolf501.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://miv.jqgufenzy.top

[Q54] 清空表
来源：http://sva.fzhhl.top

TRUNCATE TABLE logs;
来源：http://nwt.cqqwz.cn

[Q55] 排名（并列占位）
来源：http://srr.yuanzhike.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bpv.yangfankeji.com

[Q56] 密集排名（并列不占位）
来源：http://rmc.shzxlz.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dsp.yj20258.top

[Q57] 行号
来源：http://hsx.nwbrower.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cvu.wangshuangyany.cn

[Q58] 累计求和
来源：http://eks.sysykeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nzy.gzhubu.top

[Q59] 分组内累计
来源：http://hyk.ivvv.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pdd.ehwqpu.com

[Q60] 取上一行 / 下一行
来源：http://lul.snrcjt.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fvd.chenjidiqi.icu

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bbr.hysaishi.cn

[Q61] 移动平均
来源：http://dio.daxiang520.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jno.hfpthk.cn

[Q62] 分组占比
来源：http://oby.hysaishi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mdt.hywenlv.cn

[Q63] 开启事务
来源：http://hnu.nanxuanxn.top

START TRANSACTION;                -- 或 BEGIN
来源：http://isx.uphjek.com

[Q64] 提交事务
来源：http://vce.fehbvm.com

COMMIT;
来源：http://kcr.pengpengdd.cyou

[Q65] 回滚事务
来源：http://fnf.shuidangran.top

ROLLBACK;
来源：http://bbc.pengpengdd.cyou

[Q66] 行锁查询
来源：http://wdj.tian-w.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rdh.nwbrower.top

[Q67] 设置隔离级别
来源：http://kka.andypj.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hsz.ivvv.top

[Q68] 保存点
来源：http://ebs.yfazqb.com

SAVEPOINT sp1;
来源：http://ypz.hysaishi.cn

ROLLBACK TO sp1;
来源：http://ecr.zhongyouzk.top

[Q69] 查看执行计划
来源：http://ueu.zhengqikj.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ntb.wangshuangyany.cn

[Q70] 更新统计信息
来源：http://rdw.ydzc1.top

ANALYZE TABLE users;
来源：http://frh.epnwcf.com

[Q71] 查看建表语句
来源：http://vqu.ywan-chungtsiang.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pxq.wangdashe.top

[Q72] 查看索引
来源：http://hzf.ppjwa.cn

SHOW INDEX FROM users;
来源：http://rbg.xuetiantiany.cn

[Q73] 查看表状态
来源：http://twm.ctjpmb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://gsk.aizwys.cn

[Q74] 强制使用索引
来源：http://nlf.zhaomingkeji.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wew.hcnkem.com

[Q75] 日期格式化
来源：http://jgv.xylfe.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://atf.dashuyun.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tfd.meibo888.top

[Q76] 按天统计
来源：http://hpq.zhijiandao.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rec.vehdjk.com

[Q77] 时间加减
来源：http://pfu.fanxiaobao.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://abt.yueranfly.top

[Q78] 当前时间
来源：http://mhv.jinghuilouyu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cam.dashuyun.cn

[Q79] 字符串拼接
来源：http://orz.hywenlv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wto.yangfankeji.com

[Q80] 字符串截取
来源：http://ktg.jinqigfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cvd.jinqigufen.top

[Q81] 字符串替换
来源：http://djt.bbcook.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vfk.zhengqikj.top

[Q82] 字符长度与字节长度
来源：http://log.zhiwuduotai.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://psc.hfpthk.cn

[Q83] 大小写转换
来源：http://hki.daxiang520.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hbi.shangyingyoupin.top

[Q84] 去除首尾空格
来源：http://vja.guannengcc.top

SELECT TRIM(name) FROM users;
来源：http://vqb.uphjek.com

[Q85] 数值取整
来源：http://vye.ybcxt.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xlk.fehbvm.com

[Q86] 读取 JSON 字段
来源：http://xbs.fanxiaobao.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ole.c1oappe.top

[Q87] JSON 字段做条件
来源：http://hwk.guowangkeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://emt.nwbrower.top

[Q88] 行转列（条件聚合）
来源：http://txz.hysaishi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://axm.ehwqpu.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zhp.xuanzx.com

[Q89] 判断表是否存在
来源：http://ufo.ybcxt.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://met.zdqjudy.top

[Q90] 生成序号列
来源：http://ulh.0kj1m.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xfp.shzxlz.cn

================================================================================
来源：http://ilt.ybcxt.top

R. Bash 专题
来源：http://qtk.ehwqpu.com

================================================================================
来源：http://jqf.sweek.top

[R01] shebang 与严格模式
来源：http://ofs.chenlongwang.top

#!/usr/bin/env bash
来源：http://pqz.tanke756.top

set -euo pipefail
来源：http://wnw.yfazqb.com

[R02] 变量赋值与使用
来源：http://zvk.snrcjt.cn

name="Tom"; echo "$name"
来源：http://efh.sjlbkw.cn

[R03] 只读变量
来源：http://dty.kuanghao11.cn

readonly PI=3.14
来源：http://ksk.jinqigfzy.top

[R04] 位置参数
来源：http://iij.ywan-chungtsiang.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jpk.jinyuanbaomall.cn

[R05] 参数默认值
来源：http://ltc.hywenlv.cn

name="${1:-default}"
来源：http://iil.birdmap.top

[R06] 判断命令是否存在
来源：http://fjj.jinghuilouyu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eul.ivvv.top

[R07] if 判断文件
来源：http://itc.gogol.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hhi.sxryk.cn

[R08] 数值比较
来源：http://kaz.ehwqpu.com

if (( a > b )); then echo "a 更大"; fi
来源：http://myv.zhongyouzk.top

[R09] 字符串比较
来源：http://nxl.guowangkeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pad.gotoacloud.top

[R10] 正则匹配
来源：http://kxb.cheryme.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vqh.zhongyouzk.top

[R11] case 多分支
来源：http://jct.hfpthk.cn

case "$1" in
来源：http://rif.hfpthk.cn

start) echo "启动" ;;
来源：http://tpo.sufxvd.cn

stop)  echo "停止" ;;
来源：http://hbz.hcnkem.com

*)     echo "未知命令" ;;
来源：http://fer.yangfankeji.com

esac
来源：http://keo.ydjk.org.cn

[R12] for 遍历文件
来源：http://ksr.chenlongwang.top

for f in *.txt; do echo "$f"; done
来源：http://znu.guowangkeji.top

[R13] for 计数循环
来源：http://ozc.sysykeji.top

for i in {1..10}; do echo "$i"; done
来源：http://emd.hesvh.cn

[R14] C 风格 for
来源：http://umu.kuanghao11.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rwv.birdmap.top

[R15] while 逐行读文件
来源：http://jgo.zhijiandao.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kry.jianghu66.top

[R16] until 等待条件
来源：http://krx.yonumen.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cjd.ctjpmb.com

[R17] 数组定义与取值
来源：http://yyg.tianlin.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://zjx.cheryme.top

[R18] 遍历数组
来源：http://fam.uphjek.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vpm.xylfe.cn

[R19] 数组长度
来源：http://xth.ivvv.top

echo "${#arr[@]}"
来源：http://gjt.chenjidiqi.icu

[R20] 关联数组（字典）
来源：http://rxs.yfazqb.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://drx.vqdsnc.cn

[R21] 字符串长度
来源：http://nas.gotoacloud.top

echo "${#s}"
来源：http://edy.hywenlv.cn

[R22] 截取子串
来源：http://jcb.vehdjk.com

echo "${s:0:5}"
来源：http://kxs.c1oappe.top

[R23] 字符串替换
来源：http://ddj.jinqigfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ren.ppjwa.cn

[R24] 大小写转换
来源：http://fuk.jyoumei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ibi.fehbvm.com

[R25] 去后缀 / 去前缀
来源：http://ncg.redwolf501.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://xer.yuxming.cn

[R26] 命令替换
来源：http://zbw.snrcjt.cn

now=$(date +%F); echo "$now"
来源：http://gzw.xingfuxueyuan.xyz

[R27] 算术展开
来源：http://qdo.chenlongwang.top

echo $((1 + 2 * 3))
来源：http://zoh.316326.xyz

[R28] 浮点运算
来源：http://wxf.xuetiantiany.cn

echo "scale=2; 10/3" | bc
来源：http://yef.zdqjudy.top

[R29] 定义函数
来源：http://agh.yonumen.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nfc.52xcode.cn

[R30] 函数返回状态码
来源：http://etj.feifeiyinyue.top

f() { return 0; }; f || echo "失败了"
来源：http://uoa.jiagoushi.top

[R31] 局部变量
来源：http://lkm.pycfn.com

f() { local x=1; echo "$x"; }
来源：http://znp.shanyushiyangkeji.top

[R32] 参数个数校验
来源：http://wfr.ydzc1.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mht.zdbjq.cn

[R33] 捕获错误并提示行号
来源：http://vqe.yongpay.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yyq.zycfv.cn

[R34] 退出时清理
来源：http://hpf.aibaodan.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tzx.zhaomingkeji.xyz

[R35] 后台执行并等待
来源：http://nil.nanxuanxn.top

sleep 5 & pid=$!; wait "$pid"
来源：http://hje.ivvv.top

[R36] 并发执行多个任务
来源：http://xbv.yvedp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mwp.ybcxt.top

[R37] 把输出赋给变量
来源：http://wtx.jinqigfzy.top

files=$(ls -1)
来源：http://fnu.redwolf501.top

[R38] 管道串联
来源：http://vxe.smart0.xyz

cat a.txt | grep -i error | wc -l
来源：http://dqr.xziqi.cn

[R39] 重定向标准输出与错误
来源：http://cou.hnxiangtu.top

cmd > out.log 2>&1
来源：http://bkj.redwolf501.top

[R40] 追加写日志
来源：http://hop.iojbl.cn

echo "log" >> out.log
来源：http://oly.chenjidiqi.icu

[R41] 丢弃输出
来源：http://hur.havefunace.top

cmd >/dev/null 2>&1
来源：http://vys.zdbjq.cn

[R42] 输入重定向
来源：http://wjb.cucudq.cn

wc -l < a.txt
来源：http://til.sjlbkw.cn

[R43] 按名字查找文件
来源：http://gwt.wangshuangyany.cn


<!-- 参考信息 -->