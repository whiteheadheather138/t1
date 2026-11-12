代发 wailian999

CREATE TABLE users (
来源：http://jqb.zhijiandao.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mlz.hammf.cn

name VARCHAR(50) NOT NULL,
来源：http://xog.pycfn.com

email VARCHAR(100) UNIQUE,
来源：http://lir.ehwqpu.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://aum.redwolf501.top

);
来源：http://cqo.yuanzhike.top

[Q02] 创建带外键的表
来源：http://svx.zhaomingkeji.xyz

CREATE TABLE orders (
来源：http://itq.cqqwz.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oyf.xuetiantiany.cn

user_id INT NOT NULL,
来源：http://wfu.zhongyouzk.top

amount DECIMAL(10, 2),
来源：http://gjq.xuetiantiany.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lbu.jyoumei.cn

);
来源：http://szq.jlsjyb.cn

[Q03] 增加列
来源：http://xhl.tarul.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gxe.fanxiaobao.xyz

[Q04] 修改列类型
来源：http://hpa.yueranfly.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tez.cucudq.cn

[Q05] 重命名列
来源：http://wfk.xziqi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lsj.9152youxi.cn

[Q06] 删除列
来源：http://rmo.xingfuxueyuan.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://ylt.dianchejie.cn

[Q07] 删除表
来源：http://xjj.guannengcc.top

DROP TABLE IF EXISTS orders;
来源：http://ccw.yj20258.top

[Q08] 创建普通索引
来源：http://vkj.xinyue.icu

CREATE INDEX idx_users_email ON users(email);
来源：http://djl.kuanghao11.cn

[Q09] 创建唯一索引
来源：http://kkc.zhiwuduotai.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zpc.xingfuxueyuan.xyz

[Q10] 插入单行
来源：http://jqz.zdbjq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wty.jianghu66.top

[Q11] 一次插入多行
来源：http://aeu.ydjk.org.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jxk.hongshengwenyu.top

[Q12] 插入后取自增 ID
来源：http://lsy.hywenlv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lxx.zhiwuduotai.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://brp.shanyushiyangkeji.top

[Q13] 忽略重复插入
来源：http://hjy.zhijiandao.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xnp.xinyue.icu

[Q14] 存在则更新（upsert）
来源：http://huz.mhx1999.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://okv.kuanghao11.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ern.jinqigfzy.top

[Q15] 查询全部
来源：http://pyy.sjlbkw.cn

SELECT * FROM users;
来源：http://vdb.shangyingyoupin.top

[Q16] 查询指定列
来源：http://dcs.gogol.net.cn

SELECT id, name FROM users;
来源：http://hkb.ehwqpu.com

[Q17] 条件查询
来源：http://mql.zhengqikj.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jmi.tianlin.xyz

[Q18] 模糊匹配
来源：http://eqx.jinyuanbaomall.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://svq.hammf.cn

[Q19] 范围查询
来源：http://jqp.yanxiufei.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://stp.epnwcf.com

[Q20] IN 列表
来源：http://tnp.jlsjyb.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ine.havefunace.top

[Q21] 空值判断
来源：http://lod.cashguo.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mkq.cucudq.cn

[Q22] 排序
来源：http://rna.316326.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mea.shanyushiyangtech.top

[Q23] 分页
来源：http://eag.zhijiandao.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jbf.jianghu66.top

[Q24] 去重
来源：http://vfi.snrcjt.cn

SELECT DISTINCT city FROM users;
来源：http://hrg.hesvh.cn

[Q25] 只取前 N 条
来源：http://kbc.yuanzhike.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lac.xuetiantiany.cn

[Q26] 计数
来源：http://wvi.meibo888.top

SELECT COUNT(*) FROM users;
来源：http://hpc.cdnleiting.top

[Q27] 条件计数
来源：http://auj.ywan-chungtsiang.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mur.yongpay.top

[Q28] 求和与平均
来源：http://ios.hywenlv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zkr.gotoacloud.top

[Q29] 最大最小值
来源：http://znz.fzhhl.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://flu.tanke756.top

[Q30] 分组统计
来源：http://sfw.hysaishi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gkv.jianghu66.top

[Q31] 分组后过滤
来源：http://lgg.zhoulong.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://aad.uphjek.com

[Q32] 分组拼接字符串
来源：http://noi.daxiang520.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hnb.ydzc1.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kca.haohaochexian.top

[Q33] 多列分组
来源：http://qbj.aizwys.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vri.yuanzhike.top

[Q34] 每组取第一条
来源：http://kjx.yj20258888.top

SELECT * FROM (
来源：http://vur.zhaomingkeji.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bii.jinghuilouyu.cn

) t WHERE rn = 1;
来源：http://xxv.jiagoushi.top

[Q35] 内连接
来源：http://ctd.uphjek.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zmf.smart0.xyz

[Q36] 左连接
来源：http://dao.zdqjudy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vid.tianlin.xyz

[Q37] 右连接
来源：http://lhn.hcnkem.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kui.wangdashe.top

[Q38] 全外连接（PostgreSQL）
来源：http://fuu.xziqi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fcw.daxiang520.top

[Q39] 自连接（查上下级）
来源：http://vdc.jqgfzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://qov.zhaomingkeji.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ffz.yj20258.top

[Q40] 交叉连接（笛卡尔积）
来源：http://bbd.hesvh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ton.ehwqpu.com

[Q41] 多表连接
来源：http://xhu.uphjek.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://kly.snrcjt.cn

JOIN users u ON u.id = o.user_id
来源：http://hnu.chenzaomai.com

JOIN products p ON p.id = o.product_id;
来源：http://kuk.sysykeji.top

[Q42] 连接条件附加过滤
来源：http://mxx.shuidangran.top

SELECT u.name, o.amount FROM users u
来源：http://qux.dianchejie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ibf.gzhubu.top

[Q43] 标量子查询
来源：http://aod.havefunace.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ozl.tanke756.top

[Q44] IN 子查询
来源：http://ntd.pengpengdd.cyou

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xdf.sjlbkw.cn

[Q45] EXISTS 判断存在
来源：http://smb.hysaishi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ghg.shzxlz.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vvd.yj20258888.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ouc.gotoacloud.top

[Q47] 与平均值比较
来源：http://egj.chenzaomai.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ewo.zdbjq.cn

[Q48] CTE 公用表表达式
来源：http://hve.hywenlv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qkd.jinghuilouyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://eda.cashguo.top

[Q49] 更新单行
来源：http://rwy.yanxiufei.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jes.wangdashe.top

[Q50] 批量更新
来源：http://ajo.wangshuangyany.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://idi.cashguo.top

[Q51] 用子查询更新
来源：http://qqz.haohaochexian.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gex.nanxuanxn.top

[Q52] 删除指定行
来源：http://doc.fehbvm.com

DELETE FROM users WHERE id = 10;
来源：http://uti.zdqjudy.top

[Q53] 按条件删除
来源：http://exc.tian-w.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hlf.xylfe.cn

[Q54] 清空表
来源：http://xkb.kuanghao11.cn

TRUNCATE TABLE logs;
来源：http://cbf.ydjk.org.cn

[Q55] 排名（并列占位）
来源：http://hfx.dashuyun.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://miv.zhaomingkeji.xyz

[Q56] 密集排名（并列不占位）
来源：http://ipj.shangyingyoupin.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dye.guowangkeji.top

[Q57] 行号
来源：http://sxj.zhongyouzk.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mwu.yj20258.top

[Q58] 累计求和
来源：http://pmy.bjfxy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://etj.yj202588.top

[Q59] 分组内累计
来源：http://gei.vqdsnc.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pgf.tian-w.cn

[Q60] 取上一行 / 下一行
来源：http://xov.vqdsnc.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lvj.yonumen.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jiv.hesvh.cn

[Q61] 移动平均
来源：http://vnq.daria6918.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vny.xziqi.cn

[Q62] 分组占比
来源：http://ikh.yfazqb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fvd.jianghu66.top

[Q63] 开启事务
来源：http://uwd.pycfn.com

START TRANSACTION;                -- 或 BEGIN
来源：http://coq.yvedp.cn

[Q64] 提交事务
来源：http://xdt.shangyingyoupin.top

COMMIT;
来源：http://zmp.dianchejie.cn

[Q65] 回滚事务
来源：http://zfw.zhaomingkeji.xyz

ROLLBACK;
来源：http://gbw.nanxinkj.top

[Q66] 行锁查询
来源：http://ngv.fzhhl.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uen.uphjek.com

[Q67] 设置隔离级别
来源：http://gyt.vqdsnc.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dhm.ybcxt.top

[Q68] 保存点
来源：http://crm.yuanzhike.top

SAVEPOINT sp1;
来源：http://mrc.xinyue.icu

ROLLBACK TO sp1;
来源：http://qco.hongshengwenyu.top

[Q69] 查看执行计划
来源：http://otf.cqqwz.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zgs.snrcjt.cn

[Q70] 更新统计信息
来源：http://jgj.hywenlv.cn

ANALYZE TABLE users;
来源：http://cut.mhx1999.top

[Q71] 查看建表语句
来源：http://ssv.yangfankeji.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dri.yuanzhike.top

[Q72] 查看索引
来源：http://mix.mhx1999.top

SHOW INDEX FROM users;
来源：http://jwk.gaohongyu789.top

[Q73] 查看表状态
来源：http://exn.andypj.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://qdm.zdbjq.cn

[Q74] 强制使用索引
来源：http://bdx.ybcxt.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zkq.ctjpmb.com

[Q75] 日期格式化
来源：http://jyy.fktsv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xbx.dashuyun.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vqa.52xcode.cn

[Q76] 按天统计
来源：http://rqf.jinghuilouyu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://api.yanxiufei.cn

[Q77] 时间加减
来源：http://mzu.jinqigufen.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://swt.cashguo.top

[Q78] 当前时间
来源：http://cne.ybcxt.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rso.wangshuangyany.cn

[Q79] 字符串拼接
来源：http://gdw.jqgfzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oqe.aibaodan.cn

[Q80] 字符串截取
来源：http://bub.yuxming.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://isf.nanxinkj.top

[Q81] 字符串替换
来源：http://rcy.redwolf501.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wwq.zhijiandao.cn

[Q82] 字符长度与字节长度
来源：http://cho.sxryk.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://edq.ctjpmb.com

[Q83] 大小写转换
来源：http://fiq.vehdjk.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oti.gzhubu.top

[Q84] 去除首尾空格
来源：http://tei.hysaishi.cn

SELECT TRIM(name) FROM users;
来源：http://cji.jqgfzy.top

[Q85] 数值取整
来源：http://dim.xinyue.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xsy.vqdsnc.cn

[Q86] 读取 JSON 字段
来源：http://cvx.dianchejie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xrg.9152youxi.cn

[Q87] JSON 字段做条件
来源：http://jnt.sysykeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pvw.ybcxt.top

[Q88] 行转列（条件聚合）
来源：http://sdm.cashguo.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oil.hcnkem.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qrv.haohaochexian.top

[Q89] 判断表是否存在
来源：http://ows.jinghuilouyu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cir.jinyuanbaomall.cn

[Q90] 生成序号列
来源：http://ift.snrcjt.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://reu.fengsongda.top

================================================================================
来源：http://tfg.andypj.xyz

R. Bash 专题
来源：http://hwf.snrcjt.cn

================================================================================
来源：http://cen.zycfv.cn

[R01] shebang 与严格模式
来源：http://xqm.vehdjk.com

#!/usr/bin/env bash
来源：http://lky.pycfn.com

set -euo pipefail
来源：http://uys.cheryme.top

[R02] 变量赋值与使用
来源：http://jtt.zhijiandao.cn

name="Tom"; echo "$name"
来源：http://afu.ywan-chungtsiang.top

[R03] 只读变量
来源：http://kpl.chenjidiqi.icu

readonly PI=3.14
来源：http://ksj.nanxuanxn.top

[R04] 位置参数
来源：http://enb.yj20258888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cdd.mhx1999.top

[R05] 参数默认值
来源：http://gzk.ehwqpu.com

name="${1:-default}"
来源：http://ldg.cucudq.cn

[R06] 判断命令是否存在
来源：http://xpa.yj20258.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://aol.c1oappe.top

[R07] if 判断文件
来源：http://nda.cashguo.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://oiw.ywan-chungtsiang.top

[R08] 数值比较
来源：http://zew.c1oappe.top

if (( a > b )); then echo "a 更大"; fi
来源：http://jak.c1oappe.top

[R09] 字符串比较
来源：http://vpy.zhaomingkeji.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cax.yuanzhike.top

[R10] 正则匹配
来源：http://wlk.yj202588.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vdn.yj20258888.top

[R11] case 多分支
来源：http://ipi.hongshengwenyu.top

case "$1" in
来源：http://ure.316326.xyz

start) echo "启动" ;;
来源：http://xeh.haohaochexian.top

stop)  echo "停止" ;;
来源：http://zfl.yj20258.top

*)     echo "未知命令" ;;
来源：http://ibl.meibo888.top

esac
来源：http://kbc.vehdjk.com

[R12] for 遍历文件
来源：http://teo.zycfv.cn

for f in *.txt; do echo "$f"; done
来源：http://vlm.jinyuanbaomall.cn

[R13] for 计数循环
来源：http://vhs.sjlbkw.cn

for i in {1..10}; do echo "$i"; done
来源：http://oue.yvedp.cn

[R14] C 风格 for
来源：http://rlu.jyoumei.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://imb.wangshuangyany.cn

[R15] while 逐行读文件
来源：http://vbc.yongpay.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bdd.jlsjyb.cn

[R16] until 等待条件
来源：http://yto.jyoumei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dsb.tarul.cn

[R17] 数组定义与取值
来源：http://uog.cqqwz.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ajm.sjlbkw.cn

[R18] 遍历数组
来源：http://hhd.smart0.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://czk.ctjpmb.com

[R19] 数组长度
来源：http://qtw.hcnkem.com

echo "${#arr[@]}"
来源：http://mnd.jinqigfzy.top

[R20] 关联数组（字典）
来源：http://tqf.pengpengdd.cyou

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kms.shanyushiyangtech.top

[R21] 字符串长度
来源：http://bcn.jqgfzy.top

echo "${#s}"
来源：http://tes.shzxlz.cn

[R22] 截取子串
来源：http://acj.yangfankeji.com

echo "${s:0:5}"
来源：http://mug.hongshengwenyu.top

[R23] 字符串替换
来源：http://bkl.cqqwz.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pyc.fktsv.cn

[R24] 大小写转换
来源：http://jva.dashuyun.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ome.svipenyu.cn

[R25] 去后缀 / 去前缀
来源：http://yba.jinqigufen.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://uew.chenjidiqi.icu

[R26] 命令替换
来源：http://qfy.shangyingyoupin.top

now=$(date +%F); echo "$now"
来源：http://hyi.9152youxi.cn

[R27] 算术展开
来源：http://qlf.bjfxy.top

echo $((1 + 2 * 3))
来源：http://qtb.gogol.net.cn

[R28] 浮点运算
来源：http://vxh.zdbjq.cn

echo "scale=2; 10/3" | bc
来源：http://zww.smart0.xyz

[R29] 定义函数
来源：http://nig.xziqi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ifb.yj202588.top

[R30] 函数返回状态码
来源：http://gfj.daxiang520.top

f() { return 0; }; f || echo "失败了"
来源：http://ckq.gogol.net.cn

[R31] 局部变量
来源：http://sxl.sufxvd.cn

f() { local x=1; echo "$x"; }
来源：http://flr.feifeiyinyue.top

[R32] 参数个数校验
来源：http://tjw.hcnkem.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://owd.sysykeji.top

[R33] 捕获错误并提示行号
来源：http://wmf.jqgfzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tik.shanyushiyangtech.top

[R34] 退出时清理
来源：http://uvc.jianghu66.top

trap 'rm -f "$tmp"' EXIT
来源：http://qdb.daxiang520.top

[R35] 后台执行并等待
来源：http://jmp.nwbrower.top

sleep 5 & pid=$!; wait "$pid"
来源：http://lsk.tianlin.xyz

[R36] 并发执行多个任务
来源：http://ebh.ctjpmb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://smv.hysaishi.cn

[R37] 把输出赋给变量
来源：http://mwr.hysaishi.cn

files=$(ls -1)
来源：http://skv.xuetiantiany.cn

[R38] 管道串联
来源：http://lwq.ydzc1.top

cat a.txt | grep -i error | wc -l
来源：http://yzj.xinyue.icu

[R39] 重定向标准输出与错误
来源：http://azj.wangdashe.top

cmd > out.log 2>&1
来源：http://bfn.316326.xyz

[R40] 追加写日志
来源：http://znx.smart0.xyz

echo "log" >> out.log
来源：http://hbf.shanyushiyangtech.top

[R41] 丢弃输出
来源：http://dmw.birdmap.top

cmd >/dev/null 2>&1
来源：http://uhv.jinqigufen.top

[R42] 输入重定向
来源：http://xom.meibo888.top

wc -l < a.txt
来源：http://ojf.pycfn.com

[R43] 按名字查找文件
来源：http://qyi.hammf.cn

find . -name "*.log" -type f
来源：http://mty.sufxvd.cn

[R44] 按修改时间查找
来源：http://mde.jinghuilouyu.cn

find . -mtime -7 -type f
来源：http://wgy.fengsongda.top

[R45] 批量删除
来源：http://aof.ywan-chungtsiang.top


<!-- 参考信息 -->