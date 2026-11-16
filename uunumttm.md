代发 wailian999

CREATE TABLE users (
来源：http://feq.nwbrower.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rvp.quarkkingdee.top

name VARCHAR(50) NOT NULL,
来源：http://axl.jinqigufen.top

email VARCHAR(100) UNIQUE,
来源：http://pri.aibaodan.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ran.jinqigfzy.top

);
来源：http://vxy.andypj.xyz

[Q02] 创建带外键的表
来源：http://ojz.316326.xyz

CREATE TABLE orders (
来源：http://nki.pengpengdd.cyou

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rqt.cashguo.top

user_id INT NOT NULL,
来源：http://nzm.fanxiaobao.xyz

amount DECIMAL(10, 2),
来源：http://tov.ppjwa.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rna.fehbvm.com

);
来源：http://vuh.cucudq.cn

[Q03] 增加列
来源：http://ryp.nanxuanxn.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xst.xziqi.cn

[Q04] 修改列类型
来源：http://npk.vehdjk.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jjf.bbcook.cn

[Q05] 重命名列
来源：http://wra.zhongyouzk.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fae.sufxvd.cn

[Q06] 删除列
来源：http://dxi.yonumen.top

ALTER TABLE users DROP COLUMN age;
来源：http://lwh.ywan-chungtsiang.top

[Q07] 删除表
来源：http://mqo.nanxuanxn.top

DROP TABLE IF EXISTS orders;
来源：http://ncl.aizwys.cn

[Q08] 创建普通索引
来源：http://qph.shanyushiyangkeji.top

CREATE INDEX idx_users_email ON users(email);
来源：http://vjn.yfazqb.com

[Q09] 创建唯一索引
来源：http://wgn.sufxvd.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://adt.fengsongda.top

[Q10] 插入单行
来源：http://cep.nanxinkj.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cfl.xingfuxueyuan.xyz

[Q11] 一次插入多行
来源：http://lmz.hammf.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wnf.hcnkem.com

[Q12] 插入后取自增 ID
来源：http://osh.xuetiantiany.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fzp.jyoumei.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ype.guowangkeji.top

[Q13] 忽略重复插入
来源：http://mtz.shanyushiyangtech.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pvq.shanyushiyangtech.top

[Q14] 存在则更新（upsert）
来源：http://tsy.sufxvd.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uds.yuxming.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cea.jinyuanbaomall.cn

[Q15] 查询全部
来源：http://rfk.yonumen.top

SELECT * FROM users;
来源：http://yzy.xinyue.icu

[Q16] 查询指定列
来源：http://lkx.hysaishi.cn

SELECT id, name FROM users;
来源：http://iiq.yuanzhike.top

[Q17] 条件查询
来源：http://gjx.fzhhl.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cbx.hcnkem.com

[Q18] 模糊匹配
来源：http://zgp.shanyushiyangkeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zfo.zhongyouzk.top

[Q19] 范围查询
来源：http://ehr.yonumen.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blf.shzxlz.cn

[Q20] IN 列表
来源：http://tnk.redwolf501.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://csj.pycfn.com

[Q21] 空值判断
来源：http://njb.andypj.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://izz.hfpthk.cn

[Q22] 排序
来源：http://dqn.zhiwuduotai.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jke.jinqigfzy.top

[Q23] 分页
来源：http://xeo.fengsongda.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vvl.ywan-chungtsiang.top

[Q24] 去重
来源：http://cbh.xylfe.cn

SELECT DISTINCT city FROM users;
来源：http://tpm.xziqi.cn

[Q25] 只取前 N 条
来源：http://yhs.zdqjudy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://szi.hongshengwenyu.top

[Q26] 计数
来源：http://smn.zhengqikj.top

SELECT COUNT(*) FROM users;
来源：http://esc.chenzaomai.com

[Q27] 条件计数
来源：http://auv.sxryk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cnl.ppjwa.cn

[Q28] 求和与平均
来源：http://ouq.epnwcf.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vxj.jinghuilouyu.cn

[Q29] 最大最小值
来源：http://gxu.wangdashe.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://cph.yj20258888.top

[Q30] 分组统计
来源：http://xqd.vqdsnc.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://okg.hammf.cn

[Q31] 分组后过滤
来源：http://mjb.yuxming.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://aiu.cashguo.top

[Q32] 分组拼接字符串
来源：http://nbn.chenzaomai.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bxe.zhiwuduotai.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zmn.shanyushiyangkeji.top

[Q33] 多列分组
来源：http://rtf.gogol.net.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bds.yj20258.top

[Q34] 每组取第一条
来源：http://hcp.ivvv.top

SELECT * FROM (
来源：http://aaz.wangdashe.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gwa.gogol.net.cn

) t WHERE rn = 1;
来源：http://dpk.yonumen.top

[Q35] 内连接
来源：http://fug.jianghu66.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hvy.fzhhl.top

[Q36] 左连接
来源：http://fcy.jqgfzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sqv.yangfankeji.com

[Q37] 右连接
来源：http://bfi.zhengqikj.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kxz.haohaochexian.top

[Q38] 全外连接（PostgreSQL）
来源：http://wuo.zhoulong.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uye.shangyingyoupin.top

[Q39] 自连接（查上下级）
来源：http://neq.zdbjq.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ein.jyoumei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qns.c1oappe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://cvq.ctjpmb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yin.jlsjyb.cn

[Q41] 多表连接
来源：http://ofw.fehbvm.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://fsb.ydzc1.top

JOIN users u ON u.id = o.user_id
来源：http://qgn.chenlongwang.top

JOIN products p ON p.id = o.product_id;
来源：http://pot.yuxming.cn

[Q42] 连接条件附加过滤
来源：http://ytq.meibo888.top

SELECT u.name, o.amount FROM users u
来源：http://tui.c1oappe.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wie.zhoulong.xyz

[Q43] 标量子查询
来源：http://pds.9152youxi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yya.ivvv.top

[Q44] IN 子查询
来源：http://kcv.jinqigufen.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kte.xinyue.icu

[Q45] EXISTS 判断存在
来源：http://efv.yangfankeji.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://trr.hfpthk.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jkk.jinqigufen.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://asu.0kj1m.cn

[Q47] 与平均值比较
来源：http://rww.meibo888.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kkv.xylfe.cn

[Q48] CTE 公用表表达式
来源：http://nei.guannengcc.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fpr.jinqigufen.top

SELECT * FROM t WHERE c > 5;
来源：http://phf.sufxvd.cn

[Q49] 更新单行
来源：http://xzp.shanyushiyangtech.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fku.yueranfly.top

[Q50] 批量更新
来源：http://pgk.uphjek.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://slv.hnxiangtu.top

[Q51] 用子查询更新
来源：http://itx.epnwcf.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vgc.52xcode.cn

[Q52] 删除指定行
来源：http://ati.ppjwa.cn

DELETE FROM users WHERE id = 10;
来源：http://gll.aibaodan.cn

[Q53] 按条件删除
来源：http://mqi.zhongyouzk.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cmn.uphjek.com

[Q54] 清空表
来源：http://peg.yj20258.top

TRUNCATE TABLE logs;
来源：http://fry.zycfv.cn

[Q55] 排名（并列占位）
来源：http://rip.316326.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://crb.fzhhl.top

[Q56] 密集排名（并列不占位）
来源：http://geg.xylfe.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fam.zhixingplan.top

[Q57] 行号
来源：http://dqk.zdqjudy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cae.yongpay.top

[Q58] 累计求和
来源：http://jcn.yueranfly.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rxm.jinqigfzy.top

[Q59] 分组内累计
来源：http://vls.ivvv.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wyi.quarkkingdee.top

[Q60] 取上一行 / 下一行
来源：http://fgi.fktsv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sfl.jinghuilouyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ubm.cqqwz.cn

[Q61] 移动平均
来源：http://cic.316326.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jwo.fehbvm.com

[Q62] 分组占比
来源：http://jfi.shangyingyoupin.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hhe.jyoumei.cn

[Q63] 开启事务
来源：http://omu.feifeiyinyue.top

START TRANSACTION;                -- 或 BEGIN
来源：http://rhr.svipenyu.cn

[Q64] 提交事务
来源：http://uyp.ppjwa.cn

COMMIT;
来源：http://qhn.zhaomingkeji.xyz

[Q65] 回滚事务
来源：http://kom.fktsv.cn

ROLLBACK;
来源：http://gfk.fanxiaobao.xyz

[Q66] 行锁查询
来源：http://tpa.cucudq.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ehv.ehwqpu.com

[Q67] 设置隔离级别
来源：http://hqc.aibaodan.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yda.fktsv.cn

[Q68] 保存点
来源：http://jgi.gotoacloud.top

SAVEPOINT sp1;
来源：http://xhf.ybcxt.top

ROLLBACK TO sp1;
来源：http://bsz.jinyuanbaomall.cn

[Q69] 查看执行计划
来源：http://yef.sxryk.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://olx.smart0.xyz

[Q70] 更新统计信息
来源：http://aso.shzxlz.cn

ANALYZE TABLE users;
来源：http://aco.epnwcf.com

[Q71] 查看建表语句
来源：http://bvd.ywan-chungtsiang.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://url.jinghuilouyu.cn

[Q72] 查看索引
来源：http://kxz.yonumen.top

SHOW INDEX FROM users;
来源：http://cuo.cqqwz.cn

[Q73] 查看表状态
来源：http://ayz.hcnkem.com

SHOW TABLE STATUS LIKE 'users';
来源：http://gah.shangyingyoupin.top

[Q74] 强制使用索引
来源：http://bot.ybcxt.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bfe.zhongyouzk.top

[Q75] 日期格式化
来源：http://dzz.jinqigfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bzr.wangdashe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xpv.aizwys.cn

[Q76] 按天统计
来源：http://gfw.xinyue.icu

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tyh.shuidangran.top

[Q77] 时间加减
来源：http://gym.sufxvd.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kjm.hnxiangtu.top

[Q78] 当前时间
来源：http://eer.haohaochexian.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://odr.ydjk.org.cn

[Q79] 字符串拼接
来源：http://uof.fzhhl.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://flk.zhiwuduotai.top

[Q80] 字符串截取
来源：http://eqe.fengsongda.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://afa.9152youxi.cn

[Q81] 字符串替换
来源：http://lqd.gogol.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bfo.shuidangran.top

[Q82] 字符长度与字节长度
来源：http://tca.cheryme.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xud.fehbvm.com

[Q83] 大小写转换
来源：http://clt.jiagoushi.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uoe.bbcook.cn

[Q84] 去除首尾空格
来源：http://ogy.jyoumei.cn

SELECT TRIM(name) FROM users;
来源：http://uuc.pycfn.com

[Q85] 数值取整
来源：http://dqk.fengsongda.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hcv.xingfuxueyuan.xyz

[Q86] 读取 JSON 字段
来源：http://dbr.hysaishi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kqm.ywan-chungtsiang.top

[Q87] JSON 字段做条件
来源：http://ogw.snrcjt.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://khy.wangshuangyany.cn

[Q88] 行转列（条件聚合）
来源：http://htu.smart0.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tvc.cucudq.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wxg.sjlbkw.cn

[Q89] 判断表是否存在
来源：http://ybe.yj20258888.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cod.vehdjk.com

[Q90] 生成序号列
来源：http://sgf.nwbrower.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://frd.ivvv.top

================================================================================
来源：http://dsa.tianlin.xyz

R. Bash 专题
来源：http://zlq.ppjwa.cn

================================================================================
来源：http://nvf.316326.xyz

[R01] shebang 与严格模式
来源：http://itg.yvedp.cn

#!/usr/bin/env bash
来源：http://gyv.ctjpmb.com

set -euo pipefail
来源：http://kgl.sweek.top

[R02] 变量赋值与使用
来源：http://peg.fktsv.cn

name="Tom"; echo "$name"
来源：http://gvh.xuetiantiany.cn

[R03] 只读变量
来源：http://foa.hnxiangtu.top

readonly PI=3.14
来源：http://eih.xziqi.cn

[R04] 位置参数
来源：http://gbc.cashguo.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vnz.jinqigfzy.top

[R05] 参数默认值
来源：http://ogj.sjlbkw.cn

name="${1:-default}"
来源：http://rte.shzxlz.cn

[R06] 判断命令是否存在
来源：http://bnx.fanxiaobao.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mex.vqdsnc.cn

[R07] if 判断文件
来源：http://kkh.wangdashe.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zbc.hfpthk.cn

[R08] 数值比较
来源：http://ckk.tianlin.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://onp.sweek.top

[R09] 字符串比较
来源：http://mbn.redwolf501.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pjo.nwbrower.top

[R10] 正则匹配
来源：http://rpd.ybcxt.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zbr.feifeiyinyue.top

[R11] case 多分支
来源：http://koo.yangfankeji.com

case "$1" in
来源：http://guf.daria6918.cn

start) echo "启动" ;;
来源：http://ues.ehwqpu.com

stop)  echo "停止" ;;
来源：http://vyr.haohaochexian.top

*)     echo "未知命令" ;;
来源：http://chx.cucudq.cn

esac
来源：http://jxt.pengpengdd.cyou

[R12] for 遍历文件
来源：http://odc.sysykeji.top

for f in *.txt; do echo "$f"; done
来源：http://ajw.snrcjt.cn

[R13] for 计数循环
来源：http://zxn.zycfv.cn

for i in {1..10}; do echo "$i"; done
来源：http://yky.hywenlv.cn

[R14] C 风格 for
来源：http://edw.yonumen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wke.cheryme.top

[R15] while 逐行读文件
来源：http://iio.zycfv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kqt.hnxiangtu.top

[R16] until 等待条件
来源：http://rmm.hywenlv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lnb.sysykeji.top

[R17] 数组定义与取值
来源：http://are.shanyushiyangkeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://sya.aibaodan.cn

[R18] 遍历数组
来源：http://wbc.meibo888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://scm.yonumen.top

[R19] 数组长度
来源：http://zgy.yj20258.top

echo "${#arr[@]}"
来源：http://uko.zhaomingkeji.xyz

[R20] 关联数组（字典）
来源：http://nef.birdmap.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nxp.xinyue.icu

[R21] 字符串长度
来源：http://dgr.ctjpmb.com

echo "${#s}"
来源：http://onm.hfpthk.cn

[R22] 截取子串
来源：http://mut.redwolf501.top

echo "${s:0:5}"
来源：http://qjc.vqdsnc.cn

[R23] 字符串替换
来源：http://jiw.0kj1m.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://icm.fzhhl.top

[R24] 大小写转换
来源：http://aip.mhx1999.top

echo "${s^^}"; echo "${s,,}"
来源：http://yxy.svipenyu.cn

[R25] 去后缀 / 去前缀
来源：http://uvp.hcnkem.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://nfc.cashguo.top

[R26] 命令替换
来源：http://err.chenzaomai.com

now=$(date +%F); echo "$now"
来源：http://oes.xinyue.icu

[R27] 算术展开
来源：http://yhv.gotoacloud.top

echo $((1 + 2 * 3))
来源：http://sgv.aibaodan.cn

[R28] 浮点运算
来源：http://mnv.bbcook.cn

echo "scale=2; 10/3" | bc
来源：http://nzg.zhoulong.xyz

[R29] 定义函数
来源：http://jla.zdbjq.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hsb.yuxming.cn

[R30] 函数返回状态码
来源：http://skz.yvedp.cn

f() { return 0; }; f || echo "失败了"
来源：http://fcv.yueranfly.top

[R31] 局部变量
来源：http://xep.hywenlv.cn

f() { local x=1; echo "$x"; }
来源：http://oue.sjlbkw.cn

[R32] 参数个数校验
来源：http://sni.ctjpmb.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://thh.jiagoushi.top

[R33] 捕获错误并提示行号
来源：http://you.wangdashe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xkj.xinyue.icu

[R34] 退出时清理
来源：http://ipa.hammf.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rih.fktsv.cn

[R35] 后台执行并等待
来源：http://kbl.tanke756.top

sleep 5 & pid=$!; wait "$pid"
来源：http://bie.ywan-chungtsiang.top

[R36] 并发执行多个任务
来源：http://cln.ydzc1.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hui.yj20258.top

[R37] 把输出赋给变量
来源：http://zsh.yj20258.top

files=$(ls -1)
来源：http://vot.fktsv.cn

[R38] 管道串联
来源：http://mqm.quarkkingdee.top

cat a.txt | grep -i error | wc -l
来源：http://hil.kuanghao11.cn

[R39] 重定向标准输出与错误
来源：http://rak.ehwqpu.com

cmd > out.log 2>&1
来源：http://cpx.havefunace.top

[R40] 追加写日志
来源：http://opb.hywenlv.cn

echo "log" >> out.log
来源：http://kox.nanxinkj.top

[R41] 丢弃输出
来源：http://qge.epnwcf.com

cmd >/dev/null 2>&1
来源：http://efw.feifeiyinyue.top

[R42] 输入重定向
来源：http://xun.c1oappe.top

wc -l < a.txt
来源：http://vfw.hywenlv.cn

[R43] 按名字查找文件
来源：http://hvj.nwbrower.top

find . -name "*.log" -type f
来源：http://eqq.zdqjudy.top

[R44] 按修改时间查找
来源：http://evu.daria6918.cn

find . -mtime -7 -type f
来源：http://zlg.xingfuxueyuan.xyz

[R45] 批量删除
来源：http://nvu.ppjwa.cn


<!-- 参考信息 -->