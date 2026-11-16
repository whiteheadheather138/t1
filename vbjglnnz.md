代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ewf.xuanzx.com

);
来源：http://lou.52xcode.cn

[Q02] 创建带外键的表
来源：http://yed.yongpay.top

CREATE TABLE orders (
来源：http://dzk.daxiang520.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rte.uphjek.com

user_id INT NOT NULL,
来源：http://wku.fzhhl.top

amount DECIMAL(10, 2),
来源：http://hny.jyoumei.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rls.sjlbkw.cn

);
来源：http://vdg.chenjidiqi.icu

[Q03] 增加列
来源：http://qvw.snrcjt.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lft.smart0.xyz

[Q04] 修改列类型
来源：http://mmm.fengsongda.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dbt.aizwys.cn

[Q05] 重命名列
来源：http://dhc.meibo888.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vdv.mhx1999.top

[Q06] 删除列
来源：http://utb.yangfankeji.com

ALTER TABLE users DROP COLUMN age;
来源：http://jnm.birdmap.top

[Q07] 删除表
来源：http://efb.ybcxt.top

DROP TABLE IF EXISTS orders;
来源：http://ovj.bbcook.cn

[Q08] 创建普通索引
来源：http://oug.uphjek.com

CREATE INDEX idx_users_email ON users(email);
来源：http://jst.feifeiyinyue.top

[Q09] 创建唯一索引
来源：http://ibw.sysykeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lgj.andypj.xyz

[Q10] 插入单行
来源：http://yaj.yueranfly.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://krp.cqqwz.cn

[Q11] 一次插入多行
来源：http://ljx.yangfankeji.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ejh.svipenyu.cn

[Q12] 插入后取自增 ID
来源：http://rgt.gogol.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://dea.jianghu66.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kqa.yuxming.cn

[Q13] 忽略重复插入
来源：http://vlh.jinyuanbaomall.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xdk.zhaomingkeji.xyz

[Q14] 存在则更新（upsert）
来源：http://cst.yongpay.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ddy.birdmap.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lys.jyoumei.cn

[Q15] 查询全部
来源：http://bfq.hnqzz.top

SELECT * FROM users;
来源：http://nxi.hfpthk.cn

[Q16] 查询指定列
来源：http://kas.gogol.net.cn

SELECT id, name FROM users;
来源：http://pvy.hfpthk.cn

[Q17] 条件查询
来源：http://exp.yuxming.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ddr.gzhubu.top

[Q18] 模糊匹配
来源：http://dkm.yuanzhike.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jqf.pengpengdd.cyou

[Q19] 范围查询
来源：http://oho.hysaishi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fct.zhengqikj.top

[Q20] IN 列表
来源：http://vfh.jinqigfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tai.hysaishi.cn

[Q21] 空值判断
来源：http://eet.hcnkem.com

SELECT * FROM users WHERE email IS NULL;
来源：http://cmz.zdqjudy.top

[Q22] 排序
来源：http://ume.jinyuanbaomall.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qak.gotoacloud.top

[Q23] 分页
来源：http://bfm.tarul.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dwl.jiagoushi.top

[Q24] 去重
来源：http://kmj.xingfuxueyuan.xyz

SELECT DISTINCT city FROM users;
来源：http://vea.52xcode.cn

[Q25] 只取前 N 条
来源：http://qyi.ctjpmb.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://udr.smart0.xyz

[Q26] 计数
来源：http://azy.zhijiandao.cn

SELECT COUNT(*) FROM users;
来源：http://hwa.epnwcf.com

[Q27] 条件计数
来源：http://wjx.sufxvd.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qoq.yfazqb.com

[Q28] 求和与平均
来源：http://zpt.jlsjyb.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://scw.xingfuxueyuan.xyz

[Q29] 最大最小值
来源：http://dcd.pycfn.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://bnx.jinqigufen.top

[Q30] 分组统计
来源：http://szf.chenjidiqi.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vie.hammf.cn

[Q31] 分组后过滤
来源：http://mte.zhengqikj.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hfx.xziqi.cn

[Q32] 分组拼接字符串
来源：http://bri.daxiang520.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lyy.vqdsnc.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://auv.aizwys.cn

[Q33] 多列分组
来源：http://snr.smart0.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mqk.sufxvd.cn

[Q34] 每组取第一条
来源：http://wwk.ybcxt.top

SELECT * FROM (
来源：http://mvg.zycfv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cyj.bbcook.cn

) t WHERE rn = 1;
来源：http://xzw.uphjek.com

[Q35] 内连接
来源：http://hxa.ydzc1.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://eyo.haohaochexian.top

[Q36] 左连接
来源：http://wwq.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nzn.jlsjyb.cn

[Q37] 右连接
来源：http://igd.zhoulong.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://syx.yfazqb.com

[Q38] 全外连接（PostgreSQL）
来源：http://xtk.yj202588.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jcx.hesvh.cn

[Q39] 自连接（查上下级）
来源：http://bet.vqdsnc.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://css.smart0.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zzw.bjfxy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://qfo.hfpthk.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cvd.mhx1999.top

[Q41] 多表连接
来源：http://eft.nanxinkj.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ief.smart0.xyz

JOIN users u ON u.id = o.user_id
来源：http://blm.nanxinkj.top

JOIN products p ON p.id = o.product_id;
来源：http://nog.nanxuanxn.top

[Q42] 连接条件附加过滤
来源：http://pqs.shangyingyoupin.top

SELECT u.name, o.amount FROM users u
来源：http://xfb.ctjpmb.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dou.gzhubu.top

[Q43] 标量子查询
来源：http://orz.cucudq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://psx.shuidangran.top

[Q44] IN 子查询
来源：http://rtf.52xcode.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pcp.fengsongda.top

[Q45] EXISTS 判断存在
来源：http://xzp.ydjk.org.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bge.hesvh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nwi.hongshengwenyu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hvi.zhongyouzk.top

[Q47] 与平均值比较
来源：http://jro.sufxvd.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ray.aibaodan.cn

[Q48] CTE 公用表表达式
来源：http://mni.gzhubu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bwv.yvedp.cn

SELECT * FROM t WHERE c > 5;
来源：http://ytz.jinyuanbaomall.cn

[Q49] 更新单行
来源：http://kue.yangfankeji.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vfc.ywan-chungtsiang.top

[Q50] 批量更新
来源：http://lpn.tarul.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hyg.zhaomingkeji.xyz

[Q51] 用子查询更新
来源：http://sgs.iojbl.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lgg.dianchejie.cn

[Q52] 删除指定行
来源：http://afq.nanxinkj.top

DELETE FROM users WHERE id = 10;
来源：http://xsy.sufxvd.cn

[Q53] 按条件删除
来源：http://prs.daxiang520.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://czr.cucudq.cn

[Q54] 清空表
来源：http://vui.cdnleiting.top

TRUNCATE TABLE logs;
来源：http://iwg.epnwcf.com

[Q55] 排名（并列占位）
来源：http://zln.jinyuanbaomall.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://awh.fehbvm.com

[Q56] 密集排名（并列不占位）
来源：http://ksn.dashuyun.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://axj.pengpengdd.cyou

[Q57] 行号
来源：http://khc.yuanzhike.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hks.feifeiyinyue.top

[Q58] 累计求和
来源：http://ihk.epnwcf.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://krp.shanyushiyangkeji.top

[Q59] 分组内累计
来源：http://qwb.shanyushiyangtech.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zai.pycfn.com

[Q60] 取上一行 / 下一行
来源：http://sgu.jqgfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bgb.ydzc1.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://huv.xuetiantiany.cn

[Q61] 移动平均
来源：http://jau.fanxiaobao.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qzp.tarul.cn

[Q62] 分组占比
来源：http://shl.tian-w.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cdt.tianlin.xyz

[Q63] 开启事务
来源：http://vnw.jyoumei.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jni.9152youxi.cn

[Q64] 提交事务
来源：http://jqf.gogol.net.cn

COMMIT;
来源：http://fhy.feifeiyinyue.top

[Q65] 回滚事务
来源：http://ouw.gzhubu.top

ROLLBACK;
来源：http://qmr.jqgfzy.top

[Q66] 行锁查询
来源：http://qwu.guowangkeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://coo.yj20258888.top

[Q67] 设置隔离级别
来源：http://gyl.tarul.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yug.xuetiantiany.cn

[Q68] 保存点
来源：http://yds.yuxming.cn

SAVEPOINT sp1;
来源：http://cjg.tarul.cn

ROLLBACK TO sp1;
来源：http://lku.kuanghao11.cn

[Q69] 查看执行计划
来源：http://kmd.aizwys.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yzw.zdbjq.cn

[Q70] 更新统计信息
来源：http://hfh.yuxming.cn

ANALYZE TABLE users;
来源：http://bzk.sufxvd.cn

[Q71] 查看建表语句
来源：http://hhm.daxiang520.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gbi.hammf.cn

[Q72] 查看索引
来源：http://lrc.yangfankeji.com

SHOW INDEX FROM users;
来源：http://xwj.svipenyu.cn

[Q73] 查看表状态
来源：http://hgr.gzhubu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://efs.jinghuilouyu.cn

[Q74] 强制使用索引
来源：http://znw.iojbl.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xtu.cucudq.cn

[Q75] 日期格式化
来源：http://lzm.cqqwz.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rva.cucudq.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://flv.gogol.net.cn

[Q76] 按天统计
来源：http://rdv.9152youxi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xgc.vqdsnc.cn

[Q77] 时间加减
来源：http://gvb.tian-w.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://png.jlsjyb.cn

[Q78] 当前时间
来源：http://ogd.xinyue.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xrn.zycfv.cn

[Q79] 字符串拼接
来源：http://fwa.shuidangran.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tzg.0kj1m.cn

[Q80] 字符串截取
来源：http://vrv.hywenlv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://alt.jqgfzy.top

[Q81] 字符串替换
来源：http://nra.jinqigufen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zue.wangdashe.top

[Q82] 字符长度与字节长度
来源：http://wvh.feifeiyinyue.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://clw.fehbvm.com

[Q83] 大小写转换
来源：http://axw.jinghuilouyu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bbx.ehwqpu.com

[Q84] 去除首尾空格
来源：http://ekq.pengpengdd.cyou

SELECT TRIM(name) FROM users;
来源：http://wgr.xingfuxueyuan.xyz

[Q85] 数值取整
来源：http://zob.fktsv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zsu.ehwqpu.com

[Q86] 读取 JSON 字段
来源：http://vnd.yanxiufei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zpt.shanyushiyangtech.top

[Q87] JSON 字段做条件
来源：http://gel.tanke756.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://smr.chenjidiqi.icu

[Q88] 行转列（条件聚合）
来源：http://iau.tian-w.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rwq.fktsv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://etm.wangdashe.top

[Q89] 判断表是否存在
来源：http://rya.yuxming.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ylk.shuidangran.top

[Q90] 生成序号列
来源：http://gik.yj202588.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://odp.kuanghao11.cn

================================================================================
来源：http://hrh.xingfuxueyuan.xyz

R. Bash 专题
来源：http://vvw.shanyushiyangtech.top

================================================================================
来源：http://nvq.jinqigfzy.top

[R01] shebang 与严格模式
来源：http://ssp.hfpthk.cn

#!/usr/bin/env bash
来源：http://kyc.9152youxi.cn

set -euo pipefail
来源：http://stp.xingfuxueyuan.xyz

[R02] 变量赋值与使用
来源：http://wff.sjlbkw.cn

name="Tom"; echo "$name"
来源：http://xll.yangfankeji.com

[R03] 只读变量
来源：http://prs.jianghu66.top

readonly PI=3.14
来源：http://ija.pengpengdd.cyou

[R04] 位置参数
来源：http://dxz.hnqzz.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eui.hnqzz.top

[R05] 参数默认值
来源：http://eha.haohaochexian.top

name="${1:-default}"
来源：http://gxn.9152youxi.cn

[R06] 判断命令是否存在
来源：http://pbl.vqdsnc.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://msz.xziqi.cn

[R07] if 判断文件
来源：http://lbd.0kj1m.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://moo.yanxiufei.cn

[R08] 数值比较
来源：http://qyk.yongpay.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mvf.cashguo.top

[R09] 字符串比较
来源：http://bbu.ydjk.org.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://khe.cdnleiting.top

[R10] 正则匹配
来源：http://hwv.hnxiangtu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://har.zhiwuduotai.top

[R11] case 多分支
来源：http://olg.zhijiandao.cn

case "$1" in
来源：http://dma.0kj1m.cn

start) echo "启动" ;;
来源：http://uhp.wangshuangyany.cn

stop)  echo "停止" ;;
来源：http://rdx.ywan-chungtsiang.top

*)     echo "未知命令" ;;
来源：http://wfg.zhixingplan.top

esac
来源：http://pqp.sxryk.cn

[R12] for 遍历文件
来源：http://qzb.hysaishi.cn

for f in *.txt; do echo "$f"; done
来源：http://vun.jianghu66.top

[R13] for 计数循环
来源：http://den.fanxiaobao.xyz

for i in {1..10}; do echo "$i"; done
来源：http://abc.yuxming.cn

[R14] C 风格 for
来源：http://ddg.fehbvm.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vrc.fengsongda.top

[R15] while 逐行读文件
来源：http://mcy.cucudq.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ibi.ydzc1.top

[R16] until 等待条件
来源：http://imd.nwbrower.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://swj.jinqigufen.top

[R17] 数组定义与取值
来源：http://krr.yuanzhike.top

arr=(a b c); echo "${arr[0]}"
来源：http://kmo.nanxuanxn.top

[R18] 遍历数组
来源：http://sff.zhongyouzk.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bnc.chenlongwang.top

[R19] 数组长度
来源：http://xsj.0kj1m.cn

echo "${#arr[@]}"
来源：http://evm.pycfn.com

[R20] 关联数组（字典）
来源：http://kof.yongpay.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://omf.nanxuanxn.top

[R21] 字符串长度
来源：http://bbq.tarul.cn

echo "${#s}"
来源：http://uku.xziqi.cn

[R22] 截取子串
来源：http://zkb.snrcjt.cn

echo "${s:0:5}"
来源：http://vpc.feifeiyinyue.top

[R23] 字符串替换
来源：http://kth.zhengqikj.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pzu.316326.xyz

[R24] 大小写转换
来源：http://cac.guowangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://mzw.zdqjudy.top

[R25] 去后缀 / 去前缀
来源：http://xgw.zhiwuduotai.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://div.yfazqb.com

[R26] 命令替换
来源：http://not.yuxming.cn

now=$(date +%F); echo "$now"
来源：http://svh.chenjidiqi.icu

[R27] 算术展开
来源：http://amx.bjfxy.top

echo $((1 + 2 * 3))
来源：http://gjn.shanyushiyangtech.top

[R28] 浮点运算
来源：http://uin.guannengcc.top

echo "scale=2; 10/3" | bc
来源：http://isi.xuanzx.com

[R29] 定义函数
来源：http://avr.jinyuanbaomall.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xxn.sjlbkw.cn

[R30] 函数返回状态码
来源：http://tub.daxiang520.top

f() { return 0; }; f || echo "失败了"
来源：http://nuu.fehbvm.com

[R31] 局部变量
来源：http://kqv.aizwys.cn

f() { local x=1; echo "$x"; }
来源：http://dbd.yangfankeji.com

[R32] 参数个数校验
来源：http://pwr.jlsjyb.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jix.vqdsnc.cn

[R33] 捕获错误并提示行号
来源：http://ldv.9152youxi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qsn.ydzc1.top

[R34] 退出时清理
来源：http://tlb.nanxuanxn.top

trap 'rm -f "$tmp"' EXIT
来源：http://wes.meibo888.top

[R35] 后台执行并等待
来源：http://zyi.dianchejie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rju.jinyuanbaomall.cn

[R36] 并发执行多个任务
来源：http://wya.jinghuilouyu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kgw.sjlbkw.cn

[R37] 把输出赋给变量
来源：http://ubp.uphjek.com

files=$(ls -1)
来源：http://alo.meibo888.top

[R38] 管道串联
来源：http://ewh.daxiang520.top

cat a.txt | grep -i error | wc -l
来源：http://lhd.jianghu66.top

[R39] 重定向标准输出与错误
来源：http://jog.wangdashe.top

cmd > out.log 2>&1
来源：http://bam.yanxiufei.cn

[R40] 追加写日志
来源：http://obk.hammf.cn

echo "log" >> out.log
来源：http://iuh.quarkkingdee.top

[R41] 丢弃输出
来源：http://lub.gogol.net.cn

cmd >/dev/null 2>&1
来源：http://lmc.52xcode.cn

[R42] 输入重定向
来源：http://nnh.xinyue.icu

wc -l < a.txt
来源：http://alk.aizwys.cn

[R43] 按名字查找文件
来源：http://thf.feifeiyinyue.top

find . -name "*.log" -type f
来源：http://sgw.hysaishi.cn

[R44] 按修改时间查找
来源：http://krv.feifeiyinyue.top

find . -mtime -7 -type f
来源：http://ein.yuanzhike.top

[R45] 批量删除
来源：http://dfo.jinqigfzy.top

find . -name "*.tmp" -delete
来源：http://bmp.ydjk.org.cn

[R46] 递归替换文件内容
来源：http://xnf.gotoacloud.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kbc.ybcxt.top

[R47] sed 单行替换
来源：http://yjc.hesvh.cn


<!-- 参考信息 -->