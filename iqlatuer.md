代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ldu.sxryk.cn

user_id INT NOT NULL,
来源：http://bft.snrcjt.cn

amount DECIMAL(10, 2),
来源：http://qik.chenjidiqi.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tmd.sysykeji.top

);
来源：http://hqd.sysykeji.top

[Q03] 增加列
来源：http://oxt.sjlbkw.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rdp.zhijiandao.cn

[Q04] 修改列类型
来源：http://vll.hnxiangtu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sqv.guowangkeji.top

[Q05] 重命名列
来源：http://noz.wangdashe.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ppa.daxiang520.top

[Q06] 删除列
来源：http://ksk.zdqjudy.top

ALTER TABLE users DROP COLUMN age;
来源：http://xpz.sufxvd.cn

[Q07] 删除表
来源：http://cua.tianlin.xyz

DROP TABLE IF EXISTS orders;
来源：http://jyg.zycfv.cn

[Q08] 创建普通索引
来源：http://bnm.yongpay.top

CREATE INDEX idx_users_email ON users(email);
来源：http://vzg.iojbl.cn

[Q09] 创建唯一索引
来源：http://avm.shuidangran.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://byu.tian-w.cn

[Q10] 插入单行
来源：http://hiz.guowangkeji.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zmo.fktsv.cn

[Q11] 一次插入多行
来源：http://qqd.jinyuanbaomall.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lna.jiagoushi.top

[Q12] 插入后取自增 ID
来源：http://egd.ctjpmb.com

INSERT INTO users (name) VALUES ('C');
来源：http://cag.chenjidiqi.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ljh.bjfxy.top

[Q13] 忽略重复插入
来源：http://qrn.havefunace.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dvn.chenjidiqi.icu

[Q14] 存在则更新（upsert）
来源：http://vqc.birdmap.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pdl.jinyuanbaomall.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fzj.xinyue.icu

[Q15] 查询全部
来源：http://hqb.xinyue.icu

SELECT * FROM users;
来源：http://dyr.redwolf501.top

[Q16] 查询指定列
来源：http://yak.zhongyouzk.top

SELECT id, name FROM users;
来源：http://nzf.316326.xyz

[Q17] 条件查询
来源：http://wer.yj20258.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ned.redwolf501.top

[Q18] 模糊匹配
来源：http://izt.ybcxt.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rjs.hcnkem.com

[Q19] 范围查询
来源：http://agr.nanxuanxn.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vlu.shanyushiyangtech.top

[Q20] IN 列表
来源：http://skv.guowangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jno.yonumen.top

[Q21] 空值判断
来源：http://ioh.sjlbkw.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://esc.fanxiaobao.xyz

[Q22] 排序
来源：http://ubp.xinyue.icu

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fqa.ppjwa.cn

[Q23] 分页
来源：http://ghr.bbcook.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qpg.yj20258.top

[Q24] 去重
来源：http://ymk.daxiang520.top

SELECT DISTINCT city FROM users;
来源：http://heq.havefunace.top

[Q25] 只取前 N 条
来源：http://oom.zdqjudy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tav.dianchejie.cn

[Q26] 计数
来源：http://nbb.gzhubu.top

SELECT COUNT(*) FROM users;
来源：http://hlv.sweek.top

[Q27] 条件计数
来源：http://iwp.daria6918.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://eml.yvedp.cn

[Q28] 求和与平均
来源：http://soq.fehbvm.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fup.zhiwuduotai.top

[Q29] 最大最小值
来源：http://gfx.uphjek.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://tfn.tarul.cn

[Q30] 分组统计
来源：http://mgb.zhengqikj.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ozj.zhijiandao.cn

[Q31] 分组后过滤
来源：http://ero.hywenlv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vfu.sweek.top

[Q32] 分组拼接字符串
来源：http://shz.jlsjyb.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://aov.meibo888.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xqu.316326.xyz

[Q33] 多列分组
来源：http://gwi.jyoumei.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://csv.fengsongda.top

[Q34] 每组取第一条
来源：http://mzm.aibaodan.cn

SELECT * FROM (
来源：http://qoc.yfazqb.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qjx.zhijiandao.cn

) t WHERE rn = 1;
来源：http://aoc.yanxiufei.cn

[Q35] 内连接
来源：http://acw.xinyue.icu

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pwt.pycfn.com

[Q36] 左连接
来源：http://ikg.zhiwuduotai.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cmc.zhengqikj.top

[Q37] 右连接
来源：http://qcg.yj20258.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mep.shanyushiyangkeji.top

[Q38] 全外连接（PostgreSQL）
来源：http://xgn.ppjwa.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://imw.sufxvd.cn

[Q39] 自连接（查上下级）
来源：http://ala.c1oappe.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rvm.jinqigufen.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wvt.zdbjq.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://amr.cucudq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yxg.tianlin.xyz

[Q41] 多表连接
来源：http://vpf.nanxuanxn.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://iib.jqgfzy.top

JOIN users u ON u.id = o.user_id
来源：http://fiq.hnxiangtu.top

JOIN products p ON p.id = o.product_id;
来源：http://dvi.ppjwa.cn

[Q42] 连接条件附加过滤
来源：http://kre.smart0.xyz

SELECT u.name, o.amount FROM users u
来源：http://igb.pycfn.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nkj.zhoulong.xyz

[Q43] 标量子查询
来源：http://kkv.xuetiantiany.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mwo.zhongyouzk.top

[Q44] IN 子查询
来源：http://rxz.yangfankeji.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cht.yfazqb.com

[Q45] EXISTS 判断存在
来源：http://siu.yangfankeji.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zfl.havefunace.top

[Q46] NOT EXISTS 判断不存在
来源：http://pil.jinghuilouyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vmh.xingfuxueyuan.xyz

[Q47] 与平均值比较
来源：http://qlw.daxiang520.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xpy.jqgfzy.top

[Q48] CTE 公用表表达式
来源：http://epi.wangshuangyany.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://saa.xingfuxueyuan.xyz

SELECT * FROM t WHERE c > 5;
来源：http://gcd.zhoulong.xyz

[Q49] 更新单行
来源：http://mxc.uphjek.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ovx.yvedp.cn

[Q50] 批量更新
来源：http://ysh.vqdsnc.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fci.jinyuanbaomall.cn

[Q51] 用子查询更新
来源：http://wqk.smart0.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rcp.gaohongyu789.top

[Q52] 删除指定行
来源：http://mto.meibo888.top

DELETE FROM users WHERE id = 10;
来源：http://dwy.kuanghao11.cn

[Q53] 按条件删除
来源：http://sgg.xingfuxueyuan.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lxc.9152youxi.cn

[Q54] 清空表
来源：http://kxa.zhongyouzk.top

TRUNCATE TABLE logs;
来源：http://qxk.yongpay.top

[Q55] 排名（并列占位）
来源：http://uvg.yanxiufei.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ali.gzhubu.top

[Q56] 密集排名（并列不占位）
来源：http://xgb.jyoumei.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qoa.andypj.xyz

[Q57] 行号
来源：http://usk.gzhubu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dfs.jinyuanbaomall.cn

[Q58] 累计求和
来源：http://zzu.zhixingplan.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yfd.fzhhl.top

[Q59] 分组内累计
来源：http://rcj.jinyuanbaomall.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gcj.ivvv.top

[Q60] 取上一行 / 下一行
来源：http://abf.tanke756.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nxu.ywan-chungtsiang.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qhx.uphjek.com

[Q61] 移动平均
来源：http://yeq.zhoulong.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pjc.sweek.top

[Q62] 分组占比
来源：http://kyp.fanxiaobao.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ieq.sxryk.cn

[Q63] 开启事务
来源：http://bme.jiagoushi.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ibo.9152youxi.cn

[Q64] 提交事务
来源：http://rah.bbcook.cn

COMMIT;
来源：http://phr.jinghuilouyu.cn

[Q65] 回滚事务
来源：http://tkc.wangdashe.top

ROLLBACK;
来源：http://xtn.tarul.cn

[Q66] 行锁查询
来源：http://bnm.xziqi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qvb.9152youxi.cn

[Q67] 设置隔离级别
来源：http://dan.yvedp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://edy.jlsjyb.cn

[Q68] 保存点
来源：http://bne.gogol.net.cn

SAVEPOINT sp1;
来源：http://tgd.zhijiandao.cn

ROLLBACK TO sp1;
来源：http://chj.tian-w.cn

[Q69] 查看执行计划
来源：http://dnt.redwolf501.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xnm.0kj1m.cn

[Q70] 更新统计信息
来源：http://czx.hammf.cn

ANALYZE TABLE users;
来源：http://gfx.c1oappe.top

[Q71] 查看建表语句
来源：http://rhb.smart0.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jrw.sxryk.cn

[Q72] 查看索引
来源：http://dtj.ehwqpu.com

SHOW INDEX FROM users;
来源：http://hdl.0kj1m.cn

[Q73] 查看表状态
来源：http://dkx.yueranfly.top

SHOW TABLE STATUS LIKE 'users';
来源：http://dxn.gogol.net.cn

[Q74] 强制使用索引
来源：http://gra.uphjek.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://voq.zhaomingkeji.xyz

[Q75] 日期格式化
来源：http://gzu.52xcode.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cwy.xuetiantiany.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rqs.smart0.xyz

[Q76] 按天统计
来源：http://ipl.hesvh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://unj.yueranfly.top

[Q77] 时间加减
来源：http://ghq.hysaishi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kxp.jqgfzy.top

[Q78] 当前时间
来源：http://ulo.hongshengwenyu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cwj.yj20258.top

[Q79] 字符串拼接
来源：http://ect.sjlbkw.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gav.jinqigufen.top

[Q80] 字符串截取
来源：http://tes.havefunace.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uht.hesvh.cn

[Q81] 字符串替换
来源：http://tts.hongshengwenyu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://abx.cdnleiting.top

[Q82] 字符长度与字节长度
来源：http://ypz.bbcook.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uih.jinqigfzy.top

[Q83] 大小写转换
来源：http://qoa.pycfn.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cqy.jinqigfzy.top

[Q84] 去除首尾空格
来源：http://mvo.hysaishi.cn

SELECT TRIM(name) FROM users;
来源：http://mts.mhx1999.top

[Q85] 数值取整
来源：http://dxc.sysykeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pzt.cucudq.cn

[Q86] 读取 JSON 字段
来源：http://alx.aizwys.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bqz.zdqjudy.top

[Q87] JSON 字段做条件
来源：http://ctc.fzhhl.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mzo.zycfv.cn

[Q88] 行转列（条件聚合）
来源：http://wwu.hcnkem.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://frz.nanxinkj.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://iiv.iojbl.cn

[Q89] 判断表是否存在
来源：http://lxe.wangshuangyany.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://low.fktsv.cn

[Q90] 生成序号列
来源：http://xzp.fengsongda.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://quh.xingfuxueyuan.xyz

================================================================================
来源：http://qau.sxryk.cn

R. Bash 专题
来源：http://vxo.52xcode.cn

================================================================================
来源：http://xau.guowangkeji.top

[R01] shebang 与严格模式
来源：http://nni.zhongyouzk.top

#!/usr/bin/env bash
来源：http://gfn.feifeiyinyue.top

set -euo pipefail
来源：http://uqz.hnxiangtu.top

[R02] 变量赋值与使用
来源：http://tzr.xuanzx.com

name="Tom"; echo "$name"
来源：http://nhm.ivvv.top

[R03] 只读变量
来源：http://ljh.tarul.cn

readonly PI=3.14
来源：http://enn.jqgfzy.top

[R04] 位置参数
来源：http://krm.shuidangran.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wtc.yvedp.cn

[R05] 参数默认值
来源：http://azh.daria6918.cn

name="${1:-default}"
来源：http://nld.fzhhl.top

[R06] 判断命令是否存在
来源：http://nwq.iojbl.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ebo.yongpay.top

[R07] if 判断文件
来源：http://hwz.sysykeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://atp.meibo888.top

[R08] 数值比较
来源：http://hbe.gaohongyu789.top

if (( a > b )); then echo "a 更大"; fi
来源：http://iio.haohaochexian.top

[R09] 字符串比较
来源：http://frm.tian-w.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wqp.jinqigufen.top

[R10] 正则匹配
来源：http://kma.jinqigfzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zuj.cheryme.top

[R11] case 多分支
来源：http://jzc.yj20258888.top

case "$1" in
来源：http://aer.nanxinkj.top

start) echo "启动" ;;
来源：http://xab.jinyuanbaomall.cn

stop)  echo "停止" ;;
来源：http://pis.guannengcc.top

*)     echo "未知命令" ;;
来源：http://jgr.tian-w.cn

esac
来源：http://tdf.epnwcf.com

[R12] for 遍历文件
来源：http://doe.bjfxy.top

for f in *.txt; do echo "$f"; done
来源：http://zpq.xziqi.cn

[R13] for 计数循环
来源：http://kku.meibo888.top

for i in {1..10}; do echo "$i"; done
来源：http://thf.xylfe.cn

[R14] C 风格 for
来源：http://hlx.guannengcc.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tco.andypj.xyz

[R15] while 逐行读文件
来源：http://sfb.yj202588.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://myj.9152youxi.cn

[R16] until 等待条件
来源：http://jye.zhengqikj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iyr.tian-w.cn

[R17] 数组定义与取值
来源：http://gin.svipenyu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mww.vehdjk.com

[R18] 遍历数组
来源：http://ruv.ywan-chungtsiang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://skv.uphjek.com

[R19] 数组长度
来源：http://tuf.hcnkem.com

echo "${#arr[@]}"
来源：http://ica.tianlin.xyz

[R20] 关联数组（字典）
来源：http://yhg.hongshengwenyu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hgj.quarkkingdee.top

[R21] 字符串长度
来源：http://bos.tarul.cn

echo "${#s}"
来源：http://ouq.ywan-chungtsiang.top

[R22] 截取子串
来源：http://pki.jiagoushi.top

echo "${s:0:5}"
来源：http://fpv.yvedp.cn

[R23] 字符串替换
来源：http://cli.kuanghao11.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wgy.snrcjt.cn

[R24] 大小写转换
来源：http://cuy.jqgfzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://vzi.wangdashe.top

[R25] 去后缀 / 去前缀
来源：http://jat.gogol.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zap.hesvh.cn

[R26] 命令替换
来源：http://ybe.ivvv.top

now=$(date +%F); echo "$now"
来源：http://fmi.gaohongyu789.top

[R27] 算术展开
来源：http://hwc.cheryme.top

echo $((1 + 2 * 3))
来源：http://fef.hcnkem.com

[R28] 浮点运算
来源：http://ide.316326.xyz

echo "scale=2; 10/3" | bc
来源：http://pkm.ehwqpu.com

[R29] 定义函数
来源：http://lmd.shanyushiyangtech.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xth.c1oappe.top

[R30] 函数返回状态码
来源：http://qii.mhx1999.top

f() { return 0; }; f || echo "失败了"
来源：http://rnt.feifeiyinyue.top

[R31] 局部变量
来源：http://nwq.svipenyu.cn

f() { local x=1; echo "$x"; }
来源：http://smu.0kj1m.cn

[R32] 参数个数校验
来源：http://kqu.hammf.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qew.xziqi.cn

[R33] 捕获错误并提示行号
来源：http://mle.zhengqikj.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zgu.yonumen.top

[R34] 退出时清理
来源：http://thc.iojbl.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pdx.daxiang520.top

[R35] 后台执行并等待
来源：http://pab.cashguo.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xen.ppjwa.cn

[R36] 并发执行多个任务
来源：http://avr.hesvh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ocb.9152youxi.cn

[R37] 把输出赋给变量
来源：http://ifr.0kj1m.cn

files=$(ls -1)
来源：http://say.smart0.xyz

[R38] 管道串联
来源：http://sfg.shanyushiyangtech.top

cat a.txt | grep -i error | wc -l
来源：http://exm.vqdsnc.cn

[R39] 重定向标准输出与错误
来源：http://gip.zdqjudy.top

cmd > out.log 2>&1
来源：http://zru.mhx1999.top

[R40] 追加写日志
来源：http://dde.mhx1999.top

echo "log" >> out.log
来源：http://vln.kuanghao11.cn

[R41] 丢弃输出
来源：http://ysy.dianchejie.cn

cmd >/dev/null 2>&1
来源：http://jkb.redwolf501.top

[R42] 输入重定向
来源：http://unq.yongpay.top

wc -l < a.txt
来源：http://jyn.316326.xyz

[R43] 按名字查找文件
来源：http://wtw.ivvv.top

find . -name "*.log" -type f
来源：http://bfa.ppjwa.cn

[R44] 按修改时间查找
来源：http://kyn.haohaochexian.top

find . -mtime -7 -type f
来源：http://ggc.cucudq.cn

[R45] 批量删除
来源：http://wid.ppjwa.cn

find . -name "*.tmp" -delete
来源：http://czd.epnwcf.com

[R46] 递归替换文件内容
来源：http://qqw.smart0.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tvh.hcnkem.com

[R47] sed 单行替换
来源：http://vgm.jiagoushi.top

sed -i 's/foo/bar/g' a.txt
来源：http://ejk.zhixingplan.top

[R48] awk 取指定列
来源：http://oxk.chenzaomai.com

awk '{print $1, $3}' a.txt
来源：http://biq.redwolf501.top

[R49] awk 带条件
来源：http://ymo.gaohongyu789.top


<!-- 参考信息 -->