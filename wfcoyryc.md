代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xtu.tianlin.xyz

user_id INT NOT NULL,
来源：http://tyb.zhaomingkeji.xyz

amount DECIMAL(10, 2),
来源：http://qtz.yueranfly.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gab.jiagoushi.top

);
来源：http://cbn.daxiang520.top

[Q03] 增加列
来源：http://huj.sweek.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tqr.yongpay.top

[Q04] 修改列类型
来源：http://uve.cucudq.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ozk.sufxvd.cn

[Q05] 重命名列
来源：http://ugw.fengsongda.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://edj.pycfn.com

[Q06] 删除列
来源：http://rfv.9152youxi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ohb.svipenyu.cn

[Q07] 删除表
来源：http://izz.hnqzz.top

DROP TABLE IF EXISTS orders;
来源：http://qav.ctjpmb.com

[Q08] 创建普通索引
来源：http://mrj.ydjk.org.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hxt.zhiwuduotai.top

[Q09] 创建唯一索引
来源：http://ucn.yuanzhike.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nyl.chenlongwang.top

[Q10] 插入单行
来源：http://pje.yuxming.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qem.zhaomingkeji.xyz

[Q11] 一次插入多行
来源：http://zkm.yfazqb.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dya.hnqzz.top

[Q12] 插入后取自增 ID
来源：http://vxf.yj202588.top

INSERT INTO users (name) VALUES ('C');
来源：http://hic.yfazqb.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qub.dianchejie.cn

[Q13] 忽略重复插入
来源：http://mxq.quarkkingdee.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://byk.fzhhl.top

[Q14] 存在则更新（upsert）
来源：http://khn.jqgufenzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://brg.jianghu66.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kkk.shanyushiyangtech.top

[Q15] 查询全部
来源：http://uzk.yueranfly.top

SELECT * FROM users;
来源：http://kro.shuidangran.top

[Q16] 查询指定列
来源：http://url.jinghuilouyu.cn

SELECT id, name FROM users;
来源：http://ehw.yuanzhike.top

[Q17] 条件查询
来源：http://mos.yanxiufei.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xmv.sxryk.cn

[Q18] 模糊匹配
来源：http://yff.fktsv.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lgd.xziqi.cn

[Q19] 范围查询
来源：http://hjk.yj202588.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mzr.tian-w.cn

[Q20] IN 列表
来源：http://htu.tian-w.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gvg.yanxiufei.cn

[Q21] 空值判断
来源：http://isr.fanxiaobao.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://exs.zhaomingkeji.xyz

[Q22] 排序
来源：http://zpw.hcnkem.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://buu.jinyuanbaomall.cn

[Q23] 分页
来源：http://tvd.zhongyouzk.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zhm.wangdashe.top

[Q24] 去重
来源：http://vfr.ehwqpu.com

SELECT DISTINCT city FROM users;
来源：http://fbu.pycfn.com

[Q25] 只取前 N 条
来源：http://lht.316326.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mlv.zhengqikj.top

[Q26] 计数
来源：http://ssg.hesvh.cn

SELECT COUNT(*) FROM users;
来源：http://ezu.nanxuanxn.top

[Q27] 条件计数
来源：http://kcj.yvedp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uyb.zhiwuduotai.top

[Q28] 求和与平均
来源：http://nth.sweek.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rru.andypj.xyz

[Q29] 最大最小值
来源：http://maf.cdnleiting.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://edb.fengsongda.top

[Q30] 分组统计
来源：http://cnk.xziqi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jyj.birdmap.top

[Q31] 分组后过滤
来源：http://zkn.chenzaomai.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uan.zhiwuduotai.top

[Q32] 分组拼接字符串
来源：http://zfp.0kj1m.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://osx.jqgufenzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mem.yj202588.top

[Q33] 多列分组
来源：http://lcw.xingfuxueyuan.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kbr.iojbl.cn

[Q34] 每组取第一条
来源：http://qzr.feifeiyinyue.top

SELECT * FROM (
来源：http://luq.hammf.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uta.zdqjudy.top

) t WHERE rn = 1;
来源：http://lfy.daxiang520.top

[Q35] 内连接
来源：http://mcd.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jzu.vqdsnc.cn

[Q36] 左连接
来源：http://ejt.shuidangran.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zpz.redwolf501.top

[Q37] 右连接
来源：http://epu.jinqigfzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lkj.havefunace.top

[Q38] 全外连接（PostgreSQL）
来源：http://ncj.sxryk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://aiv.tarul.cn

[Q39] 自连接（查上下级）
来源：http://vrl.nanxuanxn.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ohu.yuxming.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dfv.xylfe.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ygm.c1oappe.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://szp.vqdsnc.cn

[Q41] 多表连接
来源：http://ffk.daria6918.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lci.zhiwuduotai.top

JOIN users u ON u.id = o.user_id
来源：http://qot.zhijiandao.cn

JOIN products p ON p.id = o.product_id;
来源：http://gmq.c1oappe.top

[Q42] 连接条件附加过滤
来源：http://hri.sufxvd.cn

SELECT u.name, o.amount FROM users u
来源：http://bee.cashguo.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lpl.vqdsnc.cn

[Q43] 标量子查询
来源：http://iqp.52xcode.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://avv.nanxuanxn.top

[Q44] IN 子查询
来源：http://jsh.yfazqb.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ikj.ctjpmb.com

[Q45] EXISTS 判断存在
来源：http://avw.jinyuanbaomall.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vih.dianchejie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gne.yueranfly.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ylk.xuetiantiany.cn

[Q47] 与平均值比较
来源：http://gyj.ybcxt.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ujx.guannengcc.top

[Q48] CTE 公用表表达式
来源：http://peb.feifeiyinyue.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yyu.daxiang520.top

SELECT * FROM t WHERE c > 5;
来源：http://ibf.jqgfzy.top

[Q49] 更新单行
来源：http://ibm.fzhhl.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vxq.aizwys.cn

[Q50] 批量更新
来源：http://gwg.gaohongyu789.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kwm.tarul.cn

[Q51] 用子查询更新
来源：http://esr.tianlin.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bms.snrcjt.cn

[Q52] 删除指定行
来源：http://fij.pycfn.com

DELETE FROM users WHERE id = 10;
来源：http://pyz.cashguo.top

[Q53] 按条件删除
来源：http://oua.yanxiufei.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://olq.nwbrower.top

[Q54] 清空表
来源：http://qcn.smart0.xyz

TRUNCATE TABLE logs;
来源：http://jov.xingfuxueyuan.xyz

[Q55] 排名（并列占位）
来源：http://fpv.daxiang520.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nff.iojbl.cn

[Q56] 密集排名（并列不占位）
来源：http://ujz.aibaodan.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://omu.ybcxt.top

[Q57] 行号
来源：http://hyc.xuetiantiany.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ixs.xuetiantiany.cn

[Q58] 累计求和
来源：http://fpd.ctjpmb.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xgg.gotoacloud.top

[Q59] 分组内累计
来源：http://uqh.shanyushiyangtech.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rid.dianchejie.cn

[Q60] 取上一行 / 下一行
来源：http://mcl.hywenlv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ryu.nwbrower.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gcu.sxryk.cn

[Q61] 移动平均
来源：http://dni.ywan-chungtsiang.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://atj.ppjwa.cn

[Q62] 分组占比
来源：http://lvn.vehdjk.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nvu.tianlin.xyz

[Q63] 开启事务
来源：http://mwe.316326.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://ehn.mhx1999.top

[Q64] 提交事务
来源：http://qsh.jyoumei.cn

COMMIT;
来源：http://xce.uphjek.com

[Q65] 回滚事务
来源：http://zxh.fengsongda.top

ROLLBACK;
来源：http://ite.shuidangran.top

[Q66] 行锁查询
来源：http://rlf.cdnleiting.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kuf.nanxinkj.top

[Q67] 设置隔离级别
来源：http://mfp.vqdsnc.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wft.gogol.net.cn

[Q68] 保存点
来源：http://apd.snrcjt.cn

SAVEPOINT sp1;
来源：http://djz.ybcxt.top

ROLLBACK TO sp1;
来源：http://evj.wangshuangyany.cn

[Q69] 查看执行计划
来源：http://oot.0kj1m.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://eap.sxryk.cn

[Q70] 更新统计信息
来源：http://ilp.wangshuangyany.cn

ANALYZE TABLE users;
来源：http://nbg.jinghuilouyu.cn

[Q71] 查看建表语句
来源：http://fut.jlsjyb.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://znx.jinqigufen.top

[Q72] 查看索引
来源：http://via.bbcook.cn

SHOW INDEX FROM users;
来源：http://inx.xuetiantiany.cn

[Q73] 查看表状态
来源：http://ipx.jinqigfzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://arr.zycfv.cn

[Q74] 强制使用索引
来源：http://jhb.jinqigfzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mvw.gogol.net.cn

[Q75] 日期格式化
来源：http://bja.shanyushiyangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ytx.pycfn.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://juw.hywenlv.cn

[Q76] 按天统计
来源：http://rnx.nanxuanxn.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qui.yueranfly.top

[Q77] 时间加减
来源：http://jet.vehdjk.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bnw.sweek.top

[Q78] 当前时间
来源：http://jtj.tianlin.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hnp.xziqi.cn

[Q79] 字符串拼接
来源：http://qgy.birdmap.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ghz.shanyushiyangtech.top

[Q80] 字符串截取
来源：http://biw.cqqwz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hmt.yuanzhike.top

[Q81] 字符串替换
来源：http://dip.ywan-chungtsiang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qlp.kuanghao11.cn

[Q82] 字符长度与字节长度
来源：http://ndt.jinghuilouyu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://win.jinyuanbaomall.cn

[Q83] 大小写转换
来源：http://end.yonumen.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jom.cheryme.top

[Q84] 去除首尾空格
来源：http://gwf.aizwys.cn

SELECT TRIM(name) FROM users;
来源：http://jxn.snrcjt.cn

[Q85] 数值取整
来源：http://bmz.yvedp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wbx.xylfe.cn

[Q86] 读取 JSON 字段
来源：http://czx.jinghuilouyu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kqs.0kj1m.cn

[Q87] JSON 字段做条件
来源：http://dhu.hfpthk.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rgt.cashguo.top

[Q88] 行转列（条件聚合）
来源：http://ebq.zdbjq.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xdf.bbcook.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xgq.ydjk.org.cn

[Q89] 判断表是否存在
来源：http://izz.havefunace.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vkw.aibaodan.cn

[Q90] 生成序号列
来源：http://pde.ppjwa.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ost.vqdsnc.cn

================================================================================
来源：http://xqg.hnqzz.top

R. Bash 专题
来源：http://erb.zhijiandao.cn

================================================================================
来源：http://cgi.tanke756.top

[R01] shebang 与严格模式
来源：http://kan.aibaodan.cn

#!/usr/bin/env bash
来源：http://mtd.ydjk.org.cn

set -euo pipefail
来源：http://jxn.yj20258.top

[R02] 变量赋值与使用
来源：http://haj.daxiang520.top

name="Tom"; echo "$name"
来源：http://lqb.yj20258888.top

[R03] 只读变量
来源：http://dgu.hcnkem.com

readonly PI=3.14
来源：http://pky.sxryk.cn

[R04] 位置参数
来源：http://eam.yonumen.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zed.kuanghao11.cn

[R05] 参数默认值
来源：http://ney.52xcode.cn

name="${1:-default}"
来源：http://qrt.shzxlz.cn

[R06] 判断命令是否存在
来源：http://yne.guannengcc.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cxk.cucudq.cn

[R07] if 判断文件
来源：http://iby.shzxlz.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://aud.hongshengwenyu.top

[R08] 数值比较
来源：http://heo.shanyushiyangkeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://gtg.52xcode.cn

[R09] 字符串比较
来源：http://ffh.gotoacloud.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://inx.chenjidiqi.icu

[R10] 正则匹配
来源：http://wlf.gzhubu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tub.wangshuangyany.cn

[R11] case 多分支
来源：http://kty.yangfankeji.com

case "$1" in
来源：http://efl.ctjpmb.com

start) echo "启动" ;;
来源：http://vun.jinyuanbaomall.cn

stop)  echo "停止" ;;
来源：http://pdo.hongshengwenyu.top

*)     echo "未知命令" ;;
来源：http://dhl.c1oappe.top

esac
来源：http://jlk.yuxming.cn

[R12] for 遍历文件
来源：http://poe.yongpay.top

for f in *.txt; do echo "$f"; done
来源：http://euj.hesvh.cn

[R13] for 计数循环
来源：http://wre.dashuyun.cn

for i in {1..10}; do echo "$i"; done
来源：http://qmz.vehdjk.com

[R14] C 风格 for
来源：http://toe.xylfe.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tfs.sweek.top

[R15] while 逐行读文件
来源：http://mtp.yfazqb.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hdn.9152youxi.cn

[R16] until 等待条件
来源：http://nof.nanxuanxn.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rnf.jinqigfzy.top

[R17] 数组定义与取值
来源：http://rke.kuanghao11.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ire.cucudq.cn

[R18] 遍历数组
来源：http://zdk.cdnleiting.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jqa.c1oappe.top

[R19] 数组长度
来源：http://nxl.yuanzhike.top

echo "${#arr[@]}"
来源：http://lih.sufxvd.cn

[R20] 关联数组（字典）
来源：http://wfr.zdbjq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fpp.ivvv.top

[R21] 字符串长度
来源：http://nex.jinyuanbaomall.cn

echo "${#s}"
来源：http://cno.hesvh.cn

[R22] 截取子串
来源：http://rtr.zhengqikj.top

echo "${s:0:5}"
来源：http://srm.zhijiandao.cn

[R23] 字符串替换
来源：http://qyg.xingfuxueyuan.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ubg.52xcode.cn

[R24] 大小写转换
来源：http://vsw.xinyue.icu

echo "${s^^}"; echo "${s,,}"
来源：http://znv.hysaishi.cn

[R25] 去后缀 / 去前缀
来源：http://abj.316326.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://wkd.zhijiandao.cn

[R26] 命令替换
来源：http://vox.shzxlz.cn

now=$(date +%F); echo "$now"
来源：http://fgq.vehdjk.com

[R27] 算术展开
来源：http://vyb.jqgfzy.top

echo $((1 + 2 * 3))
来源：http://tvf.xinyue.icu

[R28] 浮点运算
来源：http://qhu.wangdashe.top

echo "scale=2; 10/3" | bc
来源：http://uzu.cdnleiting.top

[R29] 定义函数
来源：http://kmh.aibaodan.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wat.havefunace.top

[R30] 函数返回状态码
来源：http://dtf.nanxuanxn.top

f() { return 0; }; f || echo "失败了"
来源：http://kos.mhx1999.top

[R31] 局部变量
来源：http://fzp.shanyushiyangkeji.top

f() { local x=1; echo "$x"; }
来源：http://ono.bbcook.cn

[R32] 参数个数校验
来源：http://goe.dianchejie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ggi.xingfuxueyuan.xyz

[R33] 捕获错误并提示行号
来源：http://raf.ydzc1.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ybr.jianghu66.top

[R34] 退出时清理
来源：http://ksu.xinyue.icu

trap 'rm -f "$tmp"' EXIT
来源：http://ifd.sjlbkw.cn

[R35] 后台执行并等待
来源：http://qnj.epnwcf.com

sleep 5 & pid=$!; wait "$pid"
来源：http://qms.fehbvm.com

[R36] 并发执行多个任务
来源：http://rhp.jinqigufen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yjj.shanyushiyangkeji.top

[R37] 把输出赋给变量
来源：http://dtx.cucudq.cn

files=$(ls -1)
来源：http://myl.zdqjudy.top

[R38] 管道串联
来源：http://kbi.yj20258.top

cat a.txt | grep -i error | wc -l
来源：http://vnk.pycfn.com

[R39] 重定向标准输出与错误
来源：http://zrj.yj20258888.top

cmd > out.log 2>&1
来源：http://ttc.ybcxt.top

[R40] 追加写日志
来源：http://dpb.xinyue.icu

echo "log" >> out.log
来源：http://uvg.cucudq.cn

[R41] 丢弃输出
来源：http://uvh.yueranfly.top

cmd >/dev/null 2>&1
来源：http://cnq.hnqzz.top

[R42] 输入重定向
来源：http://tjl.hammf.cn

wc -l < a.txt
来源：http://tot.hysaishi.cn

[R43] 按名字查找文件
来源：http://bhq.bjfxy.top

find . -name "*.log" -type f
来源：http://uvu.guannengcc.top

[R44] 按修改时间查找
来源：http://kxf.yueranfly.top

find . -mtime -7 -type f
来源：http://ogp.hywenlv.cn

[R45] 批量删除
来源：http://whv.ydjk.org.cn

find . -name "*.tmp" -delete
来源：http://lkq.jinqigfzy.top

[R46] 递归替换文件内容
来源：http://mtx.sysykeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wdd.tarul.cn

[R47] sed 单行替换
来源：http://wvf.bjfxy.top

sed -i 's/foo/bar/g' a.txt
来源：http://jko.bjfxy.top

[R48] awk 取指定列
来源：http://jhb.smart0.xyz

awk '{print $1, $3}' a.txt
来源：http://otj.jinqigufen.top

[R49] awk 带条件
来源：http://tde.cucudq.cn


<!-- 参考信息 -->