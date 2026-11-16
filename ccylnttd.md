代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dvu.jianghu66.top

);
来源：http://xdd.fktsv.cn

[Q02] 创建带外键的表
来源：http://oqg.sufxvd.cn

CREATE TABLE orders (
来源：http://zng.zdqjudy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zup.yuxming.cn

user_id INT NOT NULL,
来源：http://cce.fehbvm.com

amount DECIMAL(10, 2),
来源：http://wlp.shanyushiyangtech.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mov.jqgfzy.top

);
来源：http://fpr.yfazqb.com

[Q03] 增加列
来源：http://xob.shangyingyoupin.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pcp.xylfe.cn

[Q04] 修改列类型
来源：http://bkq.yongpay.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tak.shanyushiyangkeji.top

[Q05] 重命名列
来源：http://fsy.chenzaomai.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pfd.jqgfzy.top

[Q06] 删除列
来源：http://vpc.fengsongda.top

ALTER TABLE users DROP COLUMN age;
来源：http://soa.jianghu66.top

[Q07] 删除表
来源：http://pym.chenzaomai.com

DROP TABLE IF EXISTS orders;
来源：http://kii.shangyingyoupin.top

[Q08] 创建普通索引
来源：http://crt.hywenlv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mhd.svipenyu.cn

[Q09] 创建唯一索引
来源：http://lsy.zdqjudy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vcy.zhengqikj.top

[Q10] 插入单行
来源：http://vfe.wangshuangyany.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hxb.nanxuanxn.top

[Q11] 一次插入多行
来源：http://vvn.zdbjq.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://brv.shzxlz.cn

[Q12] 插入后取自增 ID
来源：http://qde.yuanzhike.top

INSERT INTO users (name) VALUES ('C');
来源：http://hhy.316326.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://evn.yvedp.cn

[Q13] 忽略重复插入
来源：http://qna.jinqigfzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://eep.xingfuxueyuan.xyz

[Q14] 存在则更新（upsert）
来源：http://eav.ivvv.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hpt.snrcjt.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lsy.shangyingyoupin.top

[Q15] 查询全部
来源：http://cdt.fktsv.cn

SELECT * FROM users;
来源：http://rev.yangfankeji.com

[Q16] 查询指定列
来源：http://qdn.kuanghao11.cn

SELECT id, name FROM users;
来源：http://ptl.ivvv.top

[Q17] 条件查询
来源：http://xvu.xziqi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pbv.haohaochexian.top

[Q18] 模糊匹配
来源：http://fln.pengpengdd.cyou

SELECT * FROM users WHERE name LIKE '张%';
来源：http://max.vehdjk.com

[Q19] 范围查询
来源：http://nlj.jinghuilouyu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cba.iojbl.cn

[Q20] IN 列表
来源：http://ajc.zhiwuduotai.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hli.zhijiandao.cn

[Q21] 空值判断
来源：http://hdj.yfazqb.com

SELECT * FROM users WHERE email IS NULL;
来源：http://pdk.yj20258.top

[Q22] 排序
来源：http://elv.ppjwa.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hmr.shuidangran.top

[Q23] 分页
来源：http://lwf.zhiwuduotai.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qhq.fehbvm.com

[Q24] 去重
来源：http://gvg.c1oappe.top

SELECT DISTINCT city FROM users;
来源：http://bgj.zhiwuduotai.top

[Q25] 只取前 N 条
来源：http://eho.tanke756.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uis.wangshuangyany.cn

[Q26] 计数
来源：http://bih.zhoulong.xyz

SELECT COUNT(*) FROM users;
来源：http://aum.zhixingplan.top

[Q27] 条件计数
来源：http://coe.zhiwuduotai.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jwz.havefunace.top

[Q28] 求和与平均
来源：http://hqe.chenlongwang.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qcp.gaohongyu789.top

[Q29] 最大最小值
来源：http://ksa.shzxlz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ftf.wangdashe.top

[Q30] 分组统计
来源：http://zbm.ybcxt.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://esv.yongpay.top

[Q31] 分组后过滤
来源：http://heb.dianchejie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ggd.hfpthk.cn

[Q32] 分组拼接字符串
来源：http://wbr.gzhubu.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mwb.epnwcf.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ppb.xingfuxueyuan.xyz

[Q33] 多列分组
来源：http://tpw.yueranfly.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qlb.chenjidiqi.icu

[Q34] 每组取第一条
来源：http://ygz.yvedp.cn

SELECT * FROM (
来源：http://jma.sysykeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sya.mhx1999.top

) t WHERE rn = 1;
来源：http://ves.hcnkem.com

[Q35] 内连接
来源：http://mgx.vehdjk.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bie.xinyue.icu

[Q36] 左连接
来源：http://jhb.xinyue.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ibr.kuanghao11.cn

[Q37] 右连接
来源：http://ftw.jinghuilouyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nri.birdmap.top

[Q38] 全外连接（PostgreSQL）
来源：http://zfx.bbcook.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ffq.bjfxy.top

[Q39] 自连接（查上下级）
来源：http://duo.hcnkem.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://ugu.yuanzhike.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lak.xuetiantiany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xjv.shanyushiyangtech.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://apr.guowangkeji.top

[Q41] 多表连接
来源：http://jnc.c1oappe.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://jzr.ywan-chungtsiang.top

JOIN users u ON u.id = o.user_id
来源：http://fnp.c1oappe.top

JOIN products p ON p.id = o.product_id;
来源：http://nvx.epnwcf.com

[Q42] 连接条件附加过滤
来源：http://mcb.wangdashe.top

SELECT u.name, o.amount FROM users u
来源：http://mjp.hongshengwenyu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://agm.epnwcf.com

[Q43] 标量子查询
来源：http://tet.yj202588.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ynr.jinqigufen.top

[Q44] IN 子查询
来源：http://uoz.gaohongyu789.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wit.hnxiangtu.top

[Q45] EXISTS 判断存在
来源：http://uey.jyoumei.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gbo.xuanzx.com

[Q46] NOT EXISTS 判断不存在
来源：http://wxi.gzhubu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vaw.fktsv.cn

[Q47] 与平均值比较
来源：http://mdr.ivvv.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://inf.yfazqb.com

[Q48] CTE 公用表表达式
来源：http://szz.smart0.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://foa.yuxming.cn

SELECT * FROM t WHERE c > 5;
来源：http://smd.uphjek.com

[Q49] 更新单行
来源：http://qny.dashuyun.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mci.xziqi.cn

[Q50] 批量更新
来源：http://vss.hcnkem.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://imv.yj20258888.top

[Q51] 用子查询更新
来源：http://aeq.feifeiyinyue.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hqk.zhijiandao.cn

[Q52] 删除指定行
来源：http://pcg.c1oappe.top

DELETE FROM users WHERE id = 10;
来源：http://oyx.yangfankeji.com

[Q53] 按条件删除
来源：http://aad.zycfv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ogi.0kj1m.cn

[Q54] 清空表
来源：http://yxs.jinyuanbaomall.cn

TRUNCATE TABLE logs;
来源：http://ekn.xingfuxueyuan.xyz

[Q55] 排名（并列占位）
来源：http://bos.chenjidiqi.icu

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ymo.ydzc1.top

[Q56] 密集排名（并列不占位）
来源：http://vqa.gotoacloud.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://myf.jyoumei.cn

[Q57] 行号
来源：http://ejg.ydzc1.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gya.hnxiangtu.top

[Q58] 累计求和
来源：http://wbu.c1oappe.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ljs.guannengcc.top

[Q59] 分组内累计
来源：http://csz.tianlin.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lxo.zhongyouzk.top

[Q60] 取上一行 / 下一行
来源：http://tuw.ybcxt.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://loj.c1oappe.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://srn.hywenlv.cn

[Q61] 移动平均
来源：http://fnp.pengpengdd.cyou

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hck.fanxiaobao.xyz

[Q62] 分组占比
来源：http://lau.hywenlv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zdc.mhx1999.top

[Q63] 开启事务
来源：http://tdv.xuetiantiany.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qfe.birdmap.top

[Q64] 提交事务
来源：http://ava.fengsongda.top

COMMIT;
来源：http://bdg.bbcook.cn

[Q65] 回滚事务
来源：http://tyi.xingfuxueyuan.xyz

ROLLBACK;
来源：http://vie.ehwqpu.com

[Q66] 行锁查询
来源：http://tap.dianchejie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://otd.fehbvm.com

[Q67] 设置隔离级别
来源：http://uiv.9152youxi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ats.yj20258888.top

[Q68] 保存点
来源：http://yxt.shzxlz.cn

SAVEPOINT sp1;
来源：http://nru.gzhubu.top

ROLLBACK TO sp1;
来源：http://eqy.yanxiufei.cn

[Q69] 查看执行计划
来源：http://tls.sysykeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nvi.jinyuanbaomall.cn

[Q70] 更新统计信息
来源：http://ffq.zdbjq.cn

ANALYZE TABLE users;
来源：http://vby.gzhubu.top

[Q71] 查看建表语句
来源：http://exf.havefunace.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xav.hnxiangtu.top

[Q72] 查看索引
来源：http://xni.hnxiangtu.top

SHOW INDEX FROM users;
来源：http://ipa.vehdjk.com

[Q73] 查看表状态
来源：http://dvd.sufxvd.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://yfm.tianlin.xyz

[Q74] 强制使用索引
来源：http://tbk.haohaochexian.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fzm.tian-w.cn

[Q75] 日期格式化
来源：http://clg.xuanzx.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fgj.aizwys.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://syp.jianghu66.top

[Q76] 按天统计
来源：http://imc.sysykeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://typ.aibaodan.cn

[Q77] 时间加减
来源：http://azy.wangshuangyany.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yum.jinqigfzy.top

[Q78] 当前时间
来源：http://ktd.pengpengdd.cyou

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xdp.xuanzx.com

[Q79] 字符串拼接
来源：http://xwe.zhengqikj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://als.jinqigfzy.top

[Q80] 字符串截取
来源：http://anw.pycfn.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dzu.mhx1999.top

[Q81] 字符串替换
来源：http://bzh.hfpthk.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://myq.jlsjyb.cn

[Q82] 字符长度与字节长度
来源：http://hiv.zhixingplan.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jtu.hongshengwenyu.top

[Q83] 大小写转换
来源：http://jck.vqdsnc.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xdb.yj202588.top

[Q84] 去除首尾空格
来源：http://cek.ydzc1.top

SELECT TRIM(name) FROM users;
来源：http://asy.xinyue.icu

[Q85] 数值取整
来源：http://bfw.mhx1999.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jye.zhixingplan.top

[Q86] 读取 JSON 字段
来源：http://qah.feifeiyinyue.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://riq.fehbvm.com

[Q87] JSON 字段做条件
来源：http://vkj.jqgfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ywi.chenjidiqi.icu

[Q88] 行转列（条件聚合）
来源：http://edh.epnwcf.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hbi.ydjk.org.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zdh.pycfn.com

[Q89] 判断表是否存在
来源：http://bia.hnqzz.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://txy.smart0.xyz

[Q90] 生成序号列
来源：http://plf.tanke756.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://llh.wangdashe.top

================================================================================
来源：http://qxq.ydjk.org.cn

R. Bash 专题
来源：http://rov.cqqwz.cn

================================================================================
来源：http://bxj.uphjek.com

[R01] shebang 与严格模式
来源：http://dxi.zhoulong.xyz

#!/usr/bin/env bash
来源：http://vqp.dianchejie.cn

set -euo pipefail
来源：http://anf.yuxming.cn

[R02] 变量赋值与使用
来源：http://xux.bbcook.cn

name="Tom"; echo "$name"
来源：http://xgf.jianghu66.top

[R03] 只读变量
来源：http://wgu.jianghu66.top

readonly PI=3.14
来源：http://wzq.svipenyu.cn

[R04] 位置参数
来源：http://wrc.vehdjk.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ecu.nwbrower.top

[R05] 参数默认值
来源：http://sjl.haohaochexian.top

name="${1:-default}"
来源：http://dxz.sysykeji.top

[R06] 判断命令是否存在
来源：http://dej.xinyue.icu

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wqi.yvedp.cn

[R07] if 判断文件
来源：http://mjy.wangdashe.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lyi.pycfn.com

[R08] 数值比较
来源：http://lzq.yanxiufei.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://uyz.epnwcf.com

[R09] 字符串比较
来源：http://bbs.ybcxt.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rxa.dashuyun.cn

[R10] 正则匹配
来源：http://dwq.hysaishi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fas.zycfv.cn

[R11] case 多分支
来源：http://lpm.gogol.net.cn

case "$1" in
来源：http://nxd.mhx1999.top

start) echo "启动" ;;
来源：http://ygn.hfpthk.cn

stop)  echo "停止" ;;
来源：http://tci.daria6918.cn

*)     echo "未知命令" ;;
来源：http://num.yj202588.top

esac
来源：http://blz.ctjpmb.com

[R12] for 遍历文件
来源：http://amu.52xcode.cn

for f in *.txt; do echo "$f"; done
来源：http://ocd.tian-w.cn

[R13] for 计数循环
来源：http://smb.snrcjt.cn

for i in {1..10}; do echo "$i"; done
来源：http://inx.kuanghao11.cn

[R14] C 风格 for
来源：http://tyf.havefunace.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cyj.shanyushiyangtech.top

[R15] while 逐行读文件
来源：http://ftu.yj20258.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kmh.smart0.xyz

[R16] until 等待条件
来源：http://nyu.wangdashe.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rzd.redwolf501.top

[R17] 数组定义与取值
来源：http://fhg.cdnleiting.top

arr=(a b c); echo "${arr[0]}"
来源：http://zzf.yongpay.top

[R18] 遍历数组
来源：http://rjb.ctjpmb.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://urc.meibo888.top

[R19] 数组长度
来源：http://hkr.xuanzx.com

echo "${#arr[@]}"
来源：http://oeh.birdmap.top

[R20] 关联数组（字典）
来源：http://eon.yfazqb.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://aes.chenlongwang.top

[R21] 字符串长度
来源：http://agz.cashguo.top

echo "${#s}"
来源：http://rlb.haohaochexian.top

[R22] 截取子串
来源：http://xmz.shanyushiyangtech.top

echo "${s:0:5}"
来源：http://osw.yueranfly.top

[R23] 字符串替换
来源：http://axh.hywenlv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://amv.kuanghao11.cn

[R24] 大小写转换
来源：http://krq.hywenlv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://exq.shanyushiyangkeji.top

[R25] 去后缀 / 去前缀
来源：http://fvi.fengsongda.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://eta.bjfxy.top

[R26] 命令替换
来源：http://apt.zhongyouzk.top

now=$(date +%F); echo "$now"
来源：http://anw.dianchejie.cn

[R27] 算术展开
来源：http://ail.ydzc1.top

echo $((1 + 2 * 3))
来源：http://ahg.ywan-chungtsiang.top

[R28] 浮点运算
来源：http://uok.hammf.cn

echo "scale=2; 10/3" | bc
来源：http://jli.zhongyouzk.top

[R29] 定义函数
来源：http://fku.kuanghao11.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ywb.dashuyun.cn

[R30] 函数返回状态码
来源：http://ysh.epnwcf.com

f() { return 0; }; f || echo "失败了"
来源：http://tha.zhixingplan.top

[R31] 局部变量
来源：http://myx.cdnleiting.top

f() { local x=1; echo "$x"; }
来源：http://bje.zhaomingkeji.xyz

[R32] 参数个数校验
来源：http://znv.daxiang520.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ard.sufxvd.cn

[R33] 捕获错误并提示行号
来源：http://rxb.yj20258.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yef.shangyingyoupin.top

[R34] 退出时清理
来源：http://pdk.ywan-chungtsiang.top

trap 'rm -f "$tmp"' EXIT
来源：http://fyv.fengsongda.top

[R35] 后台执行并等待
来源：http://qld.cdnleiting.top

sleep 5 & pid=$!; wait "$pid"
来源：http://flx.xuetiantiany.cn

[R36] 并发执行多个任务
来源：http://kxu.316326.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ixe.quarkkingdee.top

[R37] 把输出赋给变量
来源：http://jyu.feifeiyinyue.top

files=$(ls -1)
来源：http://crf.jianghu66.top

[R38] 管道串联
来源：http://ngw.ydjk.org.cn

cat a.txt | grep -i error | wc -l
来源：http://qpq.hesvh.cn

[R39] 重定向标准输出与错误
来源：http://xep.daxiang520.top

cmd > out.log 2>&1
来源：http://pis.gzhubu.top

[R40] 追加写日志
来源：http://ybc.zdqjudy.top

echo "log" >> out.log
来源：http://fsi.zycfv.cn

[R41] 丢弃输出
来源：http://wyx.yfazqb.com

cmd >/dev/null 2>&1
来源：http://bep.pycfn.com

[R42] 输入重定向
来源：http://que.tarul.cn

wc -l < a.txt
来源：http://pyq.tanke756.top

[R43] 按名字查找文件
来源：http://ons.c1oappe.top

find . -name "*.log" -type f
来源：http://xiu.jyoumei.cn

[R44] 按修改时间查找
来源：http://utq.ydjk.org.cn

find . -mtime -7 -type f
来源：http://gdb.jianghu66.top

[R45] 批量删除
来源：http://jwz.shanyushiyangtech.top

find . -name "*.tmp" -delete
来源：http://wfm.hysaishi.cn

[R46] 递归替换文件内容
来源：http://vvb.fktsv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://aco.yanxiufei.cn

[R47] sed 单行替换
来源：http://qkb.jlsjyb.cn


<!-- 参考信息 -->