代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uzb.ctjpmb.com

user_id INT NOT NULL,
来源：http://fej.xuanzx.com

amount DECIMAL(10, 2),
来源：http://oom.daxiang520.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fne.hysaishi.cn

);
来源：http://rwg.ehwqpu.com

[Q03] 增加列
来源：http://avj.yonumen.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ebp.daxiang520.top

[Q04] 修改列类型
来源：http://irf.hammf.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://osf.9152youxi.cn

[Q05] 重命名列
来源：http://nmc.xingfuxueyuan.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zxu.nwbrower.top

[Q06] 删除列
来源：http://eku.jinyuanbaomall.cn

ALTER TABLE users DROP COLUMN age;
来源：http://goh.wangdashe.top

[Q07] 删除表
来源：http://gjo.kuanghao11.cn

DROP TABLE IF EXISTS orders;
来源：http://hxc.bjfxy.top

[Q08] 创建普通索引
来源：http://vke.sufxvd.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://que.meibo888.top

[Q09] 创建唯一索引
来源：http://oxo.shanyushiyangtech.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qzf.yj20258.top

[Q10] 插入单行
来源：http://eql.sufxvd.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oam.svipenyu.cn

[Q11] 一次插入多行
来源：http://tiv.ywan-chungtsiang.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gzp.meibo888.top

[Q12] 插入后取自增 ID
来源：http://yoy.meibo888.top

INSERT INTO users (name) VALUES ('C');
来源：http://pqg.52xcode.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xbd.gotoacloud.top

[Q13] 忽略重复插入
来源：http://bkd.jqgfzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tmg.shanyushiyangtech.top

[Q14] 存在则更新（upsert）
来源：http://tba.fanxiaobao.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jhc.quarkkingdee.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://oye.yj20258.top

[Q15] 查询全部
来源：http://ogi.yuanzhike.top

SELECT * FROM users;
来源：http://zze.birdmap.top

[Q16] 查询指定列
来源：http://cnj.chenlongwang.top

SELECT id, name FROM users;
来源：http://fue.svipenyu.cn

[Q17] 条件查询
来源：http://whe.aibaodan.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bmn.hysaishi.cn

[Q18] 模糊匹配
来源：http://jlb.mhx1999.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ufy.bjfxy.top

[Q19] 范围查询
来源：http://lyl.ywan-chungtsiang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ovr.xinyue.icu

[Q20] IN 列表
来源：http://vkk.tianlin.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://you.zhixingplan.top

[Q21] 空值判断
来源：http://vlz.nanxinkj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mdr.gogol.net.cn

[Q22] 排序
来源：http://dxw.sxryk.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ssv.sxryk.cn

[Q23] 分页
来源：http://ekz.gaohongyu789.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://neh.nwbrower.top

[Q24] 去重
来源：http://xcw.yueranfly.top

SELECT DISTINCT city FROM users;
来源：http://nno.dashuyun.cn

[Q25] 只取前 N 条
来源：http://pzh.cheryme.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://raj.yueranfly.top

[Q26] 计数
来源：http://vmt.52xcode.cn

SELECT COUNT(*) FROM users;
来源：http://mtw.daria6918.cn

[Q27] 条件计数
来源：http://kkq.jinyuanbaomall.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dhy.hesvh.cn

[Q28] 求和与平均
来源：http://dio.tanke756.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yqc.dashuyun.cn

[Q29] 最大最小值
来源：http://hmq.dianchejie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://huq.vehdjk.com

[Q30] 分组统计
来源：http://tpq.mhx1999.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lqi.zhiwuduotai.top

[Q31] 分组后过滤
来源：http://ewj.jinghuilouyu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zbv.sweek.top

[Q32] 分组拼接字符串
来源：http://zmv.hysaishi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gub.0kj1m.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xam.jlsjyb.cn

[Q33] 多列分组
来源：http://cvi.cucudq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zur.uphjek.com

[Q34] 每组取第一条
来源：http://ywv.chenjidiqi.icu

SELECT * FROM (
来源：http://afn.xylfe.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://szn.ehwqpu.com

) t WHERE rn = 1;
来源：http://cpb.ywan-chungtsiang.top

[Q35] 内连接
来源：http://xpw.zdqjudy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gac.pycfn.com

[Q36] 左连接
来源：http://rdx.hammf.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://znf.tarul.cn

[Q37] 右连接
来源：http://ktw.shuidangran.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xrm.bjfxy.top

[Q38] 全外连接（PostgreSQL）
来源：http://bzg.pycfn.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bjv.sufxvd.cn

[Q39] 自连接（查上下级）
来源：http://saw.ctjpmb.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://pps.cqqwz.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wzi.uphjek.com

[Q40] 交叉连接（笛卡尔积）
来源：http://oyc.0kj1m.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ckm.sjlbkw.cn

[Q41] 多表连接
来源：http://crb.hnqzz.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://puo.zhongyouzk.top

JOIN users u ON u.id = o.user_id
来源：http://obh.aibaodan.cn

JOIN products p ON p.id = o.product_id;
来源：http://mfk.ivvv.top

[Q42] 连接条件附加过滤
来源：http://dll.jyoumei.cn

SELECT u.name, o.amount FROM users u
来源：http://mrt.xuanzx.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mqc.xingfuxueyuan.xyz

[Q43] 标量子查询
来源：http://xgc.tanke756.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sxc.hywenlv.cn

[Q44] IN 子查询
来源：http://nbj.ehwqpu.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rzi.ehwqpu.com

[Q45] EXISTS 判断存在
来源：http://ixe.ehwqpu.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://inc.haohaochexian.top

[Q46] NOT EXISTS 判断不存在
来源：http://snj.sufxvd.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cgr.yuxming.cn

[Q47] 与平均值比较
来源：http://vym.tanke756.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oxt.birdmap.top

[Q48] CTE 公用表表达式
来源：http://wmc.snrcjt.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nos.jinyuanbaomall.cn

SELECT * FROM t WHERE c > 5;
来源：http://qtg.sweek.top

[Q49] 更新单行
来源：http://kst.yueranfly.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://odd.vehdjk.com

[Q50] 批量更新
来源：http://cvk.daria6918.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ass.chenlongwang.top

[Q51] 用子查询更新
来源：http://xjr.cashguo.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pwn.wangdashe.top

[Q52] 删除指定行
来源：http://tyt.yongpay.top

DELETE FROM users WHERE id = 10;
来源：http://wgq.jqgfzy.top

[Q53] 按条件删除
来源：http://qtq.jqgfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://spg.ydzc1.top

[Q54] 清空表
来源：http://vyb.gotoacloud.top

TRUNCATE TABLE logs;
来源：http://nzl.pengpengdd.cyou

[Q55] 排名（并列占位）
来源：http://slg.cdnleiting.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dfa.jinghuilouyu.cn

[Q56] 密集排名（并列不占位）
来源：http://wio.zhoulong.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mai.gotoacloud.top

[Q57] 行号
来源：http://gon.nwbrower.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nzo.xziqi.cn

[Q58] 累计求和
来源：http://vzu.tian-w.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uue.gzhubu.top

[Q59] 分组内累计
来源：http://vvx.316326.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gut.uphjek.com

[Q60] 取上一行 / 下一行
来源：http://deo.xingfuxueyuan.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zfq.pycfn.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jqs.chenzaomai.com

[Q61] 移动平均
来源：http://ekq.yvedp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xmc.nanxinkj.top

[Q62] 分组占比
来源：http://esx.yj20258.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ael.hywenlv.cn

[Q63] 开启事务
来源：http://mgp.ivvv.top

START TRANSACTION;                -- 或 BEGIN
来源：http://zyv.fengsongda.top

[Q64] 提交事务
来源：http://klp.tanke756.top

COMMIT;
来源：http://def.jinqigfzy.top

[Q65] 回滚事务
来源：http://mgj.9152youxi.cn

ROLLBACK;
来源：http://jcb.shanyushiyangkeji.top

[Q66] 行锁查询
来源：http://cdu.cashguo.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gdu.fehbvm.com

[Q67] 设置隔离级别
来源：http://aft.yongpay.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lsq.hnxiangtu.top

[Q68] 保存点
来源：http://ock.cheryme.top

SAVEPOINT sp1;
来源：http://wps.yvedp.cn

ROLLBACK TO sp1;
来源：http://hux.aibaodan.cn

[Q69] 查看执行计划
来源：http://vkm.hongshengwenyu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ohh.cheryme.top

[Q70] 更新统计信息
来源：http://otk.316326.xyz

ANALYZE TABLE users;
来源：http://sql.ctjpmb.com

[Q71] 查看建表语句
来源：http://zro.tarul.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jxg.feifeiyinyue.top

[Q72] 查看索引
来源：http://cqt.vqdsnc.cn

SHOW INDEX FROM users;
来源：http://wct.9152youxi.cn

[Q73] 查看表状态
来源：http://jxv.zhijiandao.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cug.guannengcc.top

[Q74] 强制使用索引
来源：http://aab.jianghu66.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tbr.yfazqb.com

[Q75] 日期格式化
来源：http://waf.jinghuilouyu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cym.cashguo.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://iyk.tarul.cn

[Q76] 按天统计
来源：http://lvl.316326.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://msf.jinyuanbaomall.cn

[Q77] 时间加减
来源：http://jzt.aibaodan.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sdb.guowangkeji.top

[Q78] 当前时间
来源：http://lup.yj20258888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tkf.wangdashe.top

[Q79] 字符串拼接
来源：http://udl.yonumen.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ypl.nanxuanxn.top

[Q80] 字符串截取
来源：http://xtu.cashguo.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tzz.ydzc1.top

[Q81] 字符串替换
来源：http://jxs.shangyingyoupin.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gjb.chenzaomai.com

[Q82] 字符长度与字节长度
来源：http://cpl.pycfn.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yju.yueranfly.top

[Q83] 大小写转换
来源：http://izn.ywan-chungtsiang.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zdd.aizwys.cn

[Q84] 去除首尾空格
来源：http://mkz.xziqi.cn

SELECT TRIM(name) FROM users;
来源：http://dsq.ctjpmb.com

[Q85] 数值取整
来源：http://jev.hywenlv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://krz.0kj1m.cn

[Q86] 读取 JSON 字段
来源：http://pgr.yj202588.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qqh.xylfe.cn

[Q87] JSON 字段做条件
来源：http://lvq.yuanzhike.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rgh.ybcxt.top

[Q88] 行转列（条件聚合）
来源：http://xhr.jinyuanbaomall.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rlq.zhiwuduotai.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://akk.xziqi.cn

[Q89] 判断表是否存在
来源：http://nhb.9152youxi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tgq.uphjek.com

[Q90] 生成序号列
来源：http://lva.zdqjudy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://suz.jianghu66.top

================================================================================
来源：http://moe.hysaishi.cn

R. Bash 专题
来源：http://xii.9152youxi.cn

================================================================================
来源：http://cij.hongshengwenyu.top

[R01] shebang 与严格模式
来源：http://bif.jlsjyb.cn

#!/usr/bin/env bash
来源：http://tkf.sjlbkw.cn

set -euo pipefail
来源：http://jer.smart0.xyz

[R02] 变量赋值与使用
来源：http://fvy.aibaodan.cn

name="Tom"; echo "$name"
来源：http://jiy.zhijiandao.cn

[R03] 只读变量
来源：http://zou.cheryme.top

readonly PI=3.14
来源：http://col.shangyingyoupin.top

[R04] 位置参数
来源：http://okn.wangdashe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://slb.smart0.xyz

[R05] 参数默认值
来源：http://cvk.guowangkeji.top

name="${1:-default}"
来源：http://ozz.yueranfly.top

[R06] 判断命令是否存在
来源：http://teg.xuanzx.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gah.shanyushiyangtech.top

[R07] if 判断文件
来源：http://hfk.xingfuxueyuan.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sgv.guannengcc.top

[R08] 数值比较
来源：http://uon.gotoacloud.top

if (( a > b )); then echo "a 更大"; fi
来源：http://myg.hnqzz.top

[R09] 字符串比较
来源：http://yqz.yj20258.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wqj.jyoumei.cn

[R10] 正则匹配
来源：http://fhj.yj202588.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sfo.jlsjyb.cn

[R11] case 多分支
来源：http://fns.hammf.cn

case "$1" in
来源：http://lxi.zhijiandao.cn

start) echo "启动" ;;
来源：http://wpi.iojbl.cn

stop)  echo "停止" ;;
来源：http://rcf.ydjk.org.cn

*)     echo "未知命令" ;;
来源：http://yny.yvedp.cn

esac
来源：http://ajq.pengpengdd.cyou

[R12] for 遍历文件
来源：http://mjt.yongpay.top

for f in *.txt; do echo "$f"; done
来源：http://myv.sufxvd.cn

[R13] for 计数循环
来源：http://sga.sxryk.cn

for i in {1..10}; do echo "$i"; done
来源：http://dob.yj20258888.top

[R14] C 风格 for
来源：http://nes.yj20258.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://too.jinghuilouyu.cn

[R15] while 逐行读文件
来源：http://zrc.ehwqpu.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://izf.yonumen.top

[R16] until 等待条件
来源：http://vno.yvedp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jvq.ydzc1.top

[R17] 数组定义与取值
来源：http://vfh.ybcxt.top

arr=(a b c); echo "${arr[0]}"
来源：http://ivo.ivvv.top

[R18] 遍历数组
来源：http://pdq.yonumen.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://iuf.ppjwa.cn

[R19] 数组长度
来源：http://qth.hcnkem.com

echo "${#arr[@]}"
来源：http://qjt.daxiang520.top

[R20] 关联数组（字典）
来源：http://dpk.haohaochexian.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://erz.xziqi.cn

[R21] 字符串长度
来源：http://rfo.yvedp.cn

echo "${#s}"
来源：http://sgk.9152youxi.cn

[R22] 截取子串
来源：http://vks.ydjk.org.cn

echo "${s:0:5}"
来源：http://vav.bjfxy.top

[R23] 字符串替换
来源：http://okx.meibo888.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wfd.pengpengdd.cyou

[R24] 大小写转换
来源：http://lnb.smart0.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://ykn.zhiwuduotai.top

[R25] 去后缀 / 去前缀
来源：http://nsy.jinghuilouyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ncp.zhoulong.xyz

[R26] 命令替换
来源：http://hzz.yangfankeji.com

now=$(date +%F); echo "$now"
来源：http://sin.sufxvd.cn

[R27] 算术展开
来源：http://pxf.chenzaomai.com

echo $((1 + 2 * 3))
来源：http://isp.cucudq.cn

[R28] 浮点运算
来源：http://gah.jinqigufen.top

echo "scale=2; 10/3" | bc
来源：http://rjo.havefunace.top

[R29] 定义函数
来源：http://qix.jqgfzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qzz.ivvv.top

[R30] 函数返回状态码
来源：http://bpj.yuanzhike.top

f() { return 0; }; f || echo "失败了"
来源：http://etd.epnwcf.com

[R31] 局部变量
来源：http://wla.uphjek.com

f() { local x=1; echo "$x"; }
来源：http://nej.wangdashe.top

[R32] 参数个数校验
来源：http://fra.xinyue.icu

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nok.nwbrower.top

[R33] 捕获错误并提示行号
来源：http://jdq.shzxlz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mdv.hnxiangtu.top

[R34] 退出时清理
来源：http://bvm.vqdsnc.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jsu.shanyushiyangtech.top

[R35] 后台执行并等待
来源：http://tnm.yvedp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://uor.gzhubu.top

[R36] 并发执行多个任务
来源：http://plg.c1oappe.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oxh.zhiwuduotai.top

[R37] 把输出赋给变量
来源：http://ihe.zhixingplan.top

files=$(ls -1)
来源：http://hdv.sysykeji.top

[R38] 管道串联
来源：http://xwg.fzhhl.top

cat a.txt | grep -i error | wc -l
来源：http://gzf.yongpay.top

[R39] 重定向标准输出与错误
来源：http://idj.xziqi.cn

cmd > out.log 2>&1
来源：http://nlf.iojbl.cn

[R40] 追加写日志
来源：http://qpc.chenzaomai.com

echo "log" >> out.log
来源：http://uyv.cucudq.cn

[R41] 丢弃输出
来源：http://pvd.snrcjt.cn

cmd >/dev/null 2>&1
来源：http://bqh.yangfankeji.com

[R42] 输入重定向
来源：http://rxy.hcnkem.com

wc -l < a.txt
来源：http://ztc.hammf.cn

[R43] 按名字查找文件
来源：http://ljz.daria6918.cn

find . -name "*.log" -type f
来源：http://hof.hysaishi.cn

[R44] 按修改时间查找
来源：http://bky.hfpthk.cn

find . -mtime -7 -type f
来源：http://ehk.zdbjq.cn

[R45] 批量删除
来源：http://mjy.redwolf501.top

find . -name "*.tmp" -delete
来源：http://ism.9152youxi.cn

[R46] 递归替换文件内容
来源：http://kfj.ybcxt.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rhu.nanxinkj.top

[R47] sed 单行替换
来源：http://ihp.xinyue.icu

sed -i 's/foo/bar/g' a.txt
来源：http://gle.aizwys.cn

[R48] awk 取指定列
来源：http://zaf.kuanghao11.cn

awk '{print $1, $3}' a.txt
来源：http://bnp.guowangkeji.top

[R49] awk 带条件
来源：http://yxh.nanxuanxn.top


<!-- 参考信息 -->