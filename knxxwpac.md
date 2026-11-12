代发 wailian999

================================================================================
来源：http://tai.bbcook.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jik.yuanzhike.top

================================================================================
来源：http://edo.nanxuanxn.top

[Q01] 创建表
来源：http://cvo.chenzaomai.com

CREATE TABLE users (
来源：http://hsz.pengpengdd.cyou

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://edv.nanxinkj.top

name VARCHAR(50) NOT NULL,
来源：http://mjx.shanyushiyangtech.top

email VARCHAR(100) UNIQUE,
来源：http://wej.hesvh.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://foy.xingfuxueyuan.xyz

);
来源：http://kxj.cqqwz.cn

[Q02] 创建带外键的表
来源：http://kfo.tanke756.top

CREATE TABLE orders (
来源：http://zwj.yanxiufei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lou.yj202588.top

user_id INT NOT NULL,
来源：http://yzo.xuanzx.com

amount DECIMAL(10, 2),
来源：http://zga.mhx1999.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vhq.uphjek.com

);
来源：http://sxy.guannengcc.top

[Q03] 增加列
来源：http://tvw.zhaomingkeji.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wkw.nwbrower.top

[Q04] 修改列类型
来源：http://guq.sufxvd.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rbj.quarkkingdee.top

[Q05] 重命名列
来源：http://hbt.xinyue.icu

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tum.yueranfly.top

[Q06] 删除列
来源：http://hpn.zhoulong.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://tmx.gzhubu.top

[Q07] 删除表
来源：http://ovl.daria6918.cn

DROP TABLE IF EXISTS orders;
来源：http://peh.jinghuilouyu.cn

[Q08] 创建普通索引
来源：http://phg.shuidangran.top

CREATE INDEX idx_users_email ON users(email);
来源：http://wlj.jianghu66.top

[Q09] 创建唯一索引
来源：http://dxe.guannengcc.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mat.cucudq.cn

[Q10] 插入单行
来源：http://kwk.xuanzx.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bes.tanke756.top

[Q11] 一次插入多行
来源：http://tvw.smart0.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://czt.ivvv.top

[Q12] 插入后取自增 ID
来源：http://yqq.zycfv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qtt.xziqi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lzo.tarul.cn

[Q13] 忽略重复插入
来源：http://isc.jlsjyb.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xdp.pycfn.com

[Q14] 存在则更新（upsert）
来源：http://aup.jinqigufen.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rsl.fehbvm.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fmc.meibo888.top

[Q15] 查询全部
来源：http://qiy.hywenlv.cn

SELECT * FROM users;
来源：http://xvt.hywenlv.cn

[Q16] 查询指定列
来源：http://srv.sysykeji.top

SELECT id, name FROM users;
来源：http://mdd.hnxiangtu.top

[Q17] 条件查询
来源：http://hlm.iojbl.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jdl.0kj1m.cn

[Q18] 模糊匹配
来源：http://ymc.9152youxi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kmq.hfpthk.cn

[Q19] 范围查询
来源：http://hgs.sysykeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nfu.9152youxi.cn

[Q20] IN 列表
来源：http://hid.xingfuxueyuan.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://slc.gotoacloud.top

[Q21] 空值判断
来源：http://dbj.yonumen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://kil.ydzc1.top

[Q22] 排序
来源：http://opt.xuanzx.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vmo.svipenyu.cn

[Q23] 分页
来源：http://buz.zhiwuduotai.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cyy.xinyue.icu

[Q24] 去重
来源：http://ggd.sufxvd.cn

SELECT DISTINCT city FROM users;
来源：http://dyy.sysykeji.top

[Q25] 只取前 N 条
来源：http://zlf.fehbvm.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pvq.yvedp.cn

[Q26] 计数
来源：http://moh.zycfv.cn

SELECT COUNT(*) FROM users;
来源：http://sfr.9152youxi.cn

[Q27] 条件计数
来源：http://arj.haohaochexian.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ryk.epnwcf.com

[Q28] 求和与平均
来源：http://eut.hnqzz.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kpp.tian-w.cn

[Q29] 最大最小值
来源：http://wxr.52xcode.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mze.shzxlz.cn

[Q30] 分组统计
来源：http://pjh.sweek.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pdc.gzhubu.top

[Q31] 分组后过滤
来源：http://mbm.jinqigufen.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jew.9152youxi.cn

[Q32] 分组拼接字符串
来源：http://mzz.zhijiandao.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ska.sysykeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lux.nanxinkj.top

[Q33] 多列分组
来源：http://nzi.feifeiyinyue.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lxm.uphjek.com

[Q34] 每组取第一条
来源：http://ipl.dianchejie.cn

SELECT * FROM (
来源：http://ohf.tarul.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qsj.uphjek.com

) t WHERE rn = 1;
来源：http://ntp.guowangkeji.top

[Q35] 内连接
来源：http://fzs.hfpthk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rub.cdnleiting.top

[Q36] 左连接
来源：http://sve.hysaishi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://exd.aizwys.cn

[Q37] 右连接
来源：http://mso.yongpay.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kwl.jqgufenzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://reg.hywenlv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xup.yuanzhike.top

[Q39] 自连接（查上下级）
来源：http://oph.shzxlz.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://omt.hesvh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kau.fehbvm.com

[Q40] 交叉连接（笛卡尔积）
来源：http://vkt.c1oappe.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wvd.chenzaomai.com

[Q41] 多表连接
来源：http://lil.smart0.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://tun.pengpengdd.cyou

JOIN users u ON u.id = o.user_id
来源：http://axm.jinyuanbaomall.cn

JOIN products p ON p.id = o.product_id;
来源：http://ffq.hongshengwenyu.top

[Q42] 连接条件附加过滤
来源：http://myy.snrcjt.cn

SELECT u.name, o.amount FROM users u
来源：http://xwm.bbcook.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vgm.dianchejie.cn

[Q43] 标量子查询
来源：http://wxu.316326.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://icx.yongpay.top

[Q44] IN 子查询
来源：http://ygx.gaohongyu789.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://oai.wangshuangyany.cn

[Q45] EXISTS 判断存在
来源：http://trp.shanyushiyangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qsk.xuetiantiany.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zom.fanxiaobao.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wfb.yj202588.top

[Q47] 与平均值比较
来源：http://rzt.quarkkingdee.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rlo.dashuyun.cn

[Q48] CTE 公用表表达式
来源：http://xii.hysaishi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://oqv.ctjpmb.com

SELECT * FROM t WHERE c > 5;
来源：http://nwu.jlsjyb.cn

[Q49] 更新单行
来源：http://vsf.hesvh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://iba.hnxiangtu.top

[Q50] 批量更新
来源：http://zyi.jinqigufen.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lno.zhiwuduotai.top

[Q51] 用子查询更新
来源：http://wtz.c1oappe.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qiu.52xcode.cn

[Q52] 删除指定行
来源：http://mxm.daxiang520.top

DELETE FROM users WHERE id = 10;
来源：http://gzf.nanxinkj.top

[Q53] 按条件删除
来源：http://fgf.fengsongda.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dvf.jqgfzy.top

[Q54] 清空表
来源：http://pme.chenzaomai.com

TRUNCATE TABLE logs;
来源：http://dac.aizwys.cn

[Q55] 排名（并列占位）
来源：http://agl.yj20258888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gja.fzhhl.top

[Q56] 密集排名（并列不占位）
来源：http://qyo.meibo888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tib.uphjek.com

[Q57] 行号
来源：http://znm.jinyuanbaomall.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://npa.svipenyu.cn

[Q58] 累计求和
来源：http://qky.yfazqb.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lhg.yanxiufei.cn

[Q59] 分组内累计
来源：http://bxk.xuanzx.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tkc.fengsongda.top

[Q60] 取上一行 / 下一行
来源：http://rky.jinqigufen.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://puu.ydjk.org.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yms.vqdsnc.cn

[Q61] 移动平均
来源：http://mwm.shzxlz.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tdr.hesvh.cn

[Q62] 分组占比
来源：http://fhe.hcnkem.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jyh.tanke756.top

[Q63] 开启事务
来源：http://nkm.jinqigufen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gal.0kj1m.cn

[Q64] 提交事务
来源：http://yev.xinyue.icu

COMMIT;
来源：http://nsc.pycfn.com

[Q65] 回滚事务
来源：http://cqi.yanxiufei.cn

ROLLBACK;
来源：http://atw.yongpay.top

[Q66] 行锁查询
来源：http://opz.ivvv.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gly.gzhubu.top

[Q67] 设置隔离级别
来源：http://lef.hesvh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xlg.zdqjudy.top

[Q68] 保存点
来源：http://cpw.gotoacloud.top

SAVEPOINT sp1;
来源：http://amw.svipenyu.cn

ROLLBACK TO sp1;
来源：http://lxa.aizwys.cn

[Q69] 查看执行计划
来源：http://gao.cheryme.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jdt.sysykeji.top

[Q70] 更新统计信息
来源：http://gpb.pengpengdd.cyou

ANALYZE TABLE users;
来源：http://jbu.cashguo.top

[Q71] 查看建表语句
来源：http://kfm.yfazqb.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fov.zdqjudy.top

[Q72] 查看索引
来源：http://mod.yongpay.top

SHOW INDEX FROM users;
来源：http://lcu.316326.xyz

[Q73] 查看表状态
来源：http://npz.jinghuilouyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bhy.gogol.net.cn

[Q74] 强制使用索引
来源：http://nik.fehbvm.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://eog.zhijiandao.cn

[Q75] 日期格式化
来源：http://drh.hammf.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qqr.bbcook.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qhg.shanyushiyangtech.top

[Q76] 按天统计
来源：http://ioa.sufxvd.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://eaf.gotoacloud.top

[Q77] 时间加减
来源：http://nyc.9152youxi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yhg.cheryme.top

[Q78] 当前时间
来源：http://zfp.hesvh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vza.pengpengdd.cyou

[Q79] 字符串拼接
来源：http://zzs.yuxming.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gbc.sufxvd.cn

[Q80] 字符串截取
来源：http://mla.yfazqb.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://awy.chenzaomai.com

[Q81] 字符串替换
来源：http://dby.bbcook.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uif.yonumen.top

[Q82] 字符长度与字节长度
来源：http://bud.hnxiangtu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hhk.ehwqpu.com

[Q83] 大小写转换
来源：http://ouc.jyoumei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fjf.cqqwz.cn

[Q84] 去除首尾空格
来源：http://utz.yj202588.top

SELECT TRIM(name) FROM users;
来源：http://odu.shangyingyoupin.top

[Q85] 数值取整
来源：http://vfg.yj20258888.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://shn.uphjek.com

[Q86] 读取 JSON 字段
来源：http://pmf.jiagoushi.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://frv.jlsjyb.cn

[Q87] JSON 字段做条件
来源：http://jbl.daria6918.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jtc.bbcook.cn

[Q88] 行转列（条件聚合）
来源：http://qut.tian-w.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zjx.birdmap.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gwx.jlsjyb.cn

[Q89] 判断表是否存在
来源：http://cfa.jqgfzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://whf.vehdjk.com

[Q90] 生成序号列
来源：http://kgq.zhijiandao.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://oug.meibo888.top

================================================================================
来源：http://rjb.bbcook.cn

R. Bash 专题
来源：http://vom.jianghu66.top

================================================================================
来源：http://pxq.gzhubu.top

[R01] shebang 与严格模式
来源：http://vzt.cdnleiting.top

#!/usr/bin/env bash
来源：http://lnw.uphjek.com

set -euo pipefail
来源：http://fpw.mhx1999.top

[R02] 变量赋值与使用
来源：http://xcc.iojbl.cn

name="Tom"; echo "$name"
来源：http://ivt.haohaochexian.top

[R03] 只读变量
来源：http://aqg.jiagoushi.top

readonly PI=3.14
来源：http://are.zhiwuduotai.top

[R04] 位置参数
来源：http://nfz.fanxiaobao.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qiy.gaohongyu789.top

[R05] 参数默认值
来源：http://umc.yj202588.top

name="${1:-default}"
来源：http://swe.gogol.net.cn

[R06] 判断命令是否存在
来源：http://fet.bbcook.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://svq.wangshuangyany.cn

[R07] if 判断文件
来源：http://bjx.jiagoushi.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sub.jqgufenzy.top

[R08] 数值比较
来源：http://wkr.feifeiyinyue.top

if (( a > b )); then echo "a 更大"; fi
来源：http://fwr.aizwys.cn

[R09] 字符串比较
来源：http://qce.feifeiyinyue.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kei.shanyushiyangkeji.top

[R10] 正则匹配
来源：http://ekv.zdbjq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qoj.guowangkeji.top

[R11] case 多分支
来源：http://xya.hammf.cn

case "$1" in
来源：http://mig.chenzaomai.com

start) echo "启动" ;;
来源：http://qtj.svipenyu.cn

stop)  echo "停止" ;;
来源：http://gbu.chenzaomai.com

*)     echo "未知命令" ;;
来源：http://zfv.sysykeji.top

esac
来源：http://zyx.jinghuilouyu.cn

[R12] for 遍历文件
来源：http://hnf.sweek.top

for f in *.txt; do echo "$f"; done
来源：http://sye.sxryk.cn

[R13] for 计数循环
来源：http://mip.cheryme.top

for i in {1..10}; do echo "$i"; done
来源：http://bwa.jqgfzy.top

[R14] C 风格 for
来源：http://xuf.pycfn.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tuj.gzhubu.top

[R15] while 逐行读文件
来源：http://nxy.hongshengwenyu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bxi.xingfuxueyuan.xyz

[R16] until 等待条件
来源：http://xuy.tanke756.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lbm.nwbrower.top

[R17] 数组定义与取值
来源：http://que.nanxuanxn.top

arr=(a b c); echo "${arr[0]}"
来源：http://ofw.shanyushiyangkeji.top

[R18] 遍历数组
来源：http://vbq.daria6918.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ggq.dianchejie.cn

[R19] 数组长度
来源：http://uza.cdnleiting.top

echo "${#arr[@]}"
来源：http://cvy.snrcjt.cn

[R20] 关联数组（字典）
来源：http://wvn.mhx1999.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cmb.yangfankeji.com

[R21] 字符串长度
来源：http://swl.nwbrower.top

echo "${#s}"
来源：http://jbg.jiagoushi.top

[R22] 截取子串
来源：http://tnb.guannengcc.top

echo "${s:0:5}"
来源：http://qdh.zhengqikj.top

[R23] 字符串替换
来源：http://xgl.zycfv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yld.pengpengdd.cyou

[R24] 大小写转换
来源：http://njd.xinyue.icu

echo "${s^^}"; echo "${s,,}"
来源：http://doi.xingfuxueyuan.xyz

[R25] 去后缀 / 去前缀
来源：http://yvy.hywenlv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lot.pycfn.com

[R26] 命令替换
来源：http://lir.xziqi.cn

now=$(date +%F); echo "$now"
来源：http://ayq.yj202588.top

[R27] 算术展开
来源：http://gky.xylfe.cn

echo $((1 + 2 * 3))
来源：http://evb.svipenyu.cn

[R28] 浮点运算
来源：http://yzt.hammf.cn

echo "scale=2; 10/3" | bc
来源：http://dbr.gzhubu.top

[R29] 定义函数
来源：http://blf.wangshuangyany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iqc.redwolf501.top

[R30] 函数返回状态码
来源：http://bxz.fengsongda.top

f() { return 0; }; f || echo "失败了"
来源：http://eko.hysaishi.cn

[R31] 局部变量
来源：http://wma.yj20258888.top

f() { local x=1; echo "$x"; }
来源：http://nng.cashguo.top

[R32] 参数个数校验
来源：http://cae.wangshuangyany.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://okz.jlsjyb.cn

[R33] 捕获错误并提示行号
来源：http://zyp.ybcxt.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vkh.yvedp.cn

[R34] 退出时清理
来源：http://fpn.yanxiufei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://viw.sufxvd.cn

[R35] 后台执行并等待
来源：http://zzn.uphjek.com

sleep 5 & pid=$!; wait "$pid"
来源：http://syf.yuanzhike.top

[R36] 并发执行多个任务
来源：http://ytl.ehwqpu.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oaj.ivvv.top

[R37] 把输出赋给变量
来源：http://lhi.yj20258.top

files=$(ls -1)
来源：http://jig.yuanzhike.top

[R38] 管道串联
来源：http://thl.shzxlz.cn

cat a.txt | grep -i error | wc -l
来源：http://krw.cucudq.cn

[R39] 重定向标准输出与错误
来源：http://eiy.ctjpmb.com

cmd > out.log 2>&1
来源：http://szn.hysaishi.cn

[R40] 追加写日志
来源：http://dey.jinghuilouyu.cn

echo "log" >> out.log
来源：http://npk.jqgfzy.top

[R41] 丢弃输出
来源：http://ies.yangfankeji.com

cmd >/dev/null 2>&1
来源：http://rps.zhoulong.xyz

[R42] 输入重定向
来源：http://dqt.tian-w.cn

wc -l < a.txt
来源：http://hyc.bjfxy.top

[R43] 按名字查找文件
来源：http://gjf.gzhubu.top


<!-- 参考信息 -->