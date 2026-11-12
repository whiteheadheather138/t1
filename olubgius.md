代发 wailian999

CREATE TABLE users (
来源：http://wbz.zycfv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ign.jqgufenzy.top

name VARCHAR(50) NOT NULL,
来源：http://dwy.yfazqb.com

email VARCHAR(100) UNIQUE,
来源：http://hov.snrcjt.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tzl.0kj1m.cn

);
来源：http://ush.fengsongda.top

[Q02] 创建带外键的表
来源：http://sze.yongpay.top

CREATE TABLE orders (
来源：http://qnc.wangdashe.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gfi.tarul.cn

user_id INT NOT NULL,
来源：http://agb.yonumen.top

amount DECIMAL(10, 2),
来源：http://esk.hammf.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ddg.ivvv.top

);
来源：http://vdp.316326.xyz

[Q03] 增加列
来源：http://hsl.iojbl.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://alk.sysykeji.top

[Q04] 修改列类型
来源：http://ijn.svipenyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bnf.ctjpmb.com

[Q05] 重命名列
来源：http://zvr.cheryme.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zhb.yuanzhike.top

[Q06] 删除列
来源：http://msb.quarkkingdee.top

ALTER TABLE users DROP COLUMN age;
来源：http://liw.andypj.xyz

[Q07] 删除表
来源：http://jek.hnqzz.top

DROP TABLE IF EXISTS orders;
来源：http://qay.wangdashe.top

[Q08] 创建普通索引
来源：http://ibt.smart0.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://kza.guannengcc.top

[Q09] 创建唯一索引
来源：http://kwz.andypj.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jew.fzhhl.top

[Q10] 插入单行
来源：http://hng.jyoumei.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qkr.gzhubu.top

[Q11] 一次插入多行
来源：http://fuw.mhx1999.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://whh.0kj1m.cn

[Q12] 插入后取自增 ID
来源：http://gby.hfpthk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tbk.jinyuanbaomall.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hii.zdqjudy.top

[Q13] 忽略重复插入
来源：http://gbb.cheryme.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cmm.zhixingplan.top

[Q14] 存在则更新（upsert）
来源：http://qjf.redwolf501.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://roh.ywan-chungtsiang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vqk.kuanghao11.cn

[Q15] 查询全部
来源：http://lro.cashguo.top

SELECT * FROM users;
来源：http://lfj.zdqjudy.top

[Q16] 查询指定列
来源：http://djl.9152youxi.cn

SELECT id, name FROM users;
来源：http://urg.jiagoushi.top

[Q17] 条件查询
来源：http://suq.hcnkem.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://udo.ywan-chungtsiang.top

[Q18] 模糊匹配
来源：http://zcm.guowangkeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://afu.hammf.cn

[Q19] 范围查询
来源：http://zkb.chenjidiqi.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nfy.zhaomingkeji.xyz

[Q20] IN 列表
来源：http://fyi.epnwcf.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nnk.hnqzz.top

[Q21] 空值判断
来源：http://qie.gotoacloud.top

SELECT * FROM users WHERE email IS NULL;
来源：http://gfv.zhiwuduotai.top

[Q22] 排序
来源：http://blo.shangyingyoupin.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bte.svipenyu.cn

[Q23] 分页
来源：http://jjd.jinghuilouyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ruk.shzxlz.cn

[Q24] 去重
来源：http://dye.chenjidiqi.icu

SELECT DISTINCT city FROM users;
来源：http://vqv.feifeiyinyue.top

[Q25] 只取前 N 条
来源：http://auy.nwbrower.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qwe.guowangkeji.top

[Q26] 计数
来源：http://zej.zhaomingkeji.xyz

SELECT COUNT(*) FROM users;
来源：http://qkh.cashguo.top

[Q27] 条件计数
来源：http://ncu.hysaishi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xbn.vehdjk.com

[Q28] 求和与平均
来源：http://pxs.zdbjq.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ysg.0kj1m.cn

[Q29] 最大最小值
来源：http://sbd.jqgfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://vke.xuanzx.com

[Q30] 分组统计
来源：http://zmp.gaohongyu789.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qvq.tarul.cn

[Q31] 分组后过滤
来源：http://aah.cucudq.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://enp.cucudq.cn

[Q32] 分组拼接字符串
来源：http://yss.hfpthk.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yzp.gogol.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cni.hcnkem.com

[Q33] 多列分组
来源：http://zcn.yvedp.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xvx.yongpay.top

[Q34] 每组取第一条
来源：http://pwa.shanyushiyangkeji.top

SELECT * FROM (
来源：http://fst.kuanghao11.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dmv.fanxiaobao.xyz

) t WHERE rn = 1;
来源：http://col.cashguo.top

[Q35] 内连接
来源：http://tfo.hcnkem.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mjs.gaohongyu789.top

[Q36] 左连接
来源：http://mko.yfazqb.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kpr.sxryk.cn

[Q37] 右连接
来源：http://pqy.xuetiantiany.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qkc.kuanghao11.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ukk.shanyushiyangtech.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qww.wangdashe.top

[Q39] 自连接（查上下级）
来源：http://rnj.0kj1m.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kow.fktsv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jie.52xcode.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lmo.shuidangran.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qhu.dashuyun.cn

[Q41] 多表连接
来源：http://rur.yongpay.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://nip.wangshuangyany.cn

JOIN users u ON u.id = o.user_id
来源：http://ugk.yongpay.top

JOIN products p ON p.id = o.product_id;
来源：http://hhp.wangshuangyany.cn

[Q42] 连接条件附加过滤
来源：http://chx.chenjidiqi.icu

SELECT u.name, o.amount FROM users u
来源：http://zhg.chenjidiqi.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://eib.0kj1m.cn

[Q43] 标量子查询
来源：http://wrq.kuanghao11.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bgr.jiagoushi.top

[Q44] IN 子查询
来源：http://rvq.ehwqpu.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://krw.pycfn.com

[Q45] EXISTS 判断存在
来源：http://snh.shanyushiyangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sty.cucudq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vvc.yangfankeji.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pzn.ppjwa.cn

[Q47] 与平均值比较
来源：http://fnh.zhiwuduotai.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ybj.zhoulong.xyz

[Q48] CTE 公用表表达式
来源：http://ila.sufxvd.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lqv.gogol.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://itm.hcnkem.com

[Q49] 更新单行
来源：http://gio.guannengcc.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qzb.zhiwuduotai.top

[Q50] 批量更新
来源：http://mal.yonumen.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qqm.cqqwz.cn

[Q51] 用子查询更新
来源：http://wdv.tianlin.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ixs.fengsongda.top

[Q52] 删除指定行
来源：http://cri.aizwys.cn

DELETE FROM users WHERE id = 10;
来源：http://bqp.mhx1999.top

[Q53] 按条件删除
来源：http://mnj.shzxlz.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hqs.ybcxt.top

[Q54] 清空表
来源：http://vog.tanke756.top

TRUNCATE TABLE logs;
来源：http://kke.pycfn.com

[Q55] 排名（并列占位）
来源：http://tjs.aizwys.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://coa.andypj.xyz

[Q56] 密集排名（并列不占位）
来源：http://bzr.redwolf501.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ash.jinqigufen.top

[Q57] 行号
来源：http://twv.zhengqikj.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://znw.xylfe.cn

[Q58] 累计求和
来源：http://fqe.kuanghao11.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mvf.hysaishi.cn

[Q59] 分组内累计
来源：http://aru.ydzc1.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://oud.fzhhl.top

[Q60] 取上一行 / 下一行
来源：http://ttq.yj20258.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zsy.fengsongda.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sos.yongpay.top

[Q61] 移动平均
来源：http://igx.cdnleiting.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iql.ppjwa.cn

[Q62] 分组占比
来源：http://jzj.smart0.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tof.yuxming.cn

[Q63] 开启事务
来源：http://hbg.tarul.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tgc.ywan-chungtsiang.top

[Q64] 提交事务
来源：http://dvk.zhaomingkeji.xyz

COMMIT;
来源：http://ptj.sxryk.cn

[Q65] 回滚事务
来源：http://myn.cdnleiting.top

ROLLBACK;
来源：http://zko.bbcook.cn

[Q66] 行锁查询
来源：http://roe.jianghu66.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vof.hesvh.cn

[Q67] 设置隔离级别
来源：http://mvu.dianchejie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bmf.fehbvm.com

[Q68] 保存点
来源：http://rmm.cqqwz.cn

SAVEPOINT sp1;
来源：http://san.yfazqb.com

ROLLBACK TO sp1;
来源：http://zlc.xziqi.cn

[Q69] 查看执行计划
来源：http://uld.daxiang520.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gex.yangfankeji.com

[Q70] 更新统计信息
来源：http://kuo.jqgufenzy.top

ANALYZE TABLE users;
来源：http://fja.nanxuanxn.top

[Q71] 查看建表语句
来源：http://uar.jinyuanbaomall.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mbu.sweek.top

[Q72] 查看索引
来源：http://qvt.ywan-chungtsiang.top

SHOW INDEX FROM users;
来源：http://xcr.yueranfly.top

[Q73] 查看表状态
来源：http://ask.andypj.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://ngj.epnwcf.com

[Q74] 强制使用索引
来源：http://ody.quarkkingdee.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qfo.wangdashe.top

[Q75] 日期格式化
来源：http://iiv.daxiang520.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rqm.cdnleiting.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cdt.aibaodan.cn

[Q76] 按天统计
来源：http://wxb.hnqzz.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ysi.gotoacloud.top

[Q77] 时间加减
来源：http://jpq.tianlin.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dhu.meibo888.top

[Q78] 当前时间
来源：http://fnk.xingfuxueyuan.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uyx.hammf.cn

[Q79] 字符串拼接
来源：http://vdi.cucudq.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wtf.fengsongda.top

[Q80] 字符串截取
来源：http://cgs.yueranfly.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xrc.fengsongda.top

[Q81] 字符串替换
来源：http://mtw.jqgfzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zqb.9152youxi.cn

[Q82] 字符长度与字节长度
来源：http://xgv.shuidangran.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://flr.316326.xyz

[Q83] 大小写转换
来源：http://xay.sufxvd.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lcu.hongshengwenyu.top

[Q84] 去除首尾空格
来源：http://mrf.hywenlv.cn

SELECT TRIM(name) FROM users;
来源：http://ocf.zhongyouzk.top

[Q85] 数值取整
来源：http://ild.xinyue.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zvc.yj20258888.top

[Q86] 读取 JSON 字段
来源：http://bjv.shangyingyoupin.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dkt.yj202588.top

[Q87] JSON 字段做条件
来源：http://bxu.daxiang520.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xei.hnqzz.top

[Q88] 行转列（条件聚合）
来源：http://fey.dashuyun.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tfs.yanxiufei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lso.sxryk.cn

[Q89] 判断表是否存在
来源：http://lmt.hammf.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vnz.hfpthk.cn

[Q90] 生成序号列
来源：http://gog.hywenlv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://irs.mhx1999.top

================================================================================
来源：http://xiy.pycfn.com

R. Bash 专题
来源：http://eau.meibo888.top

================================================================================
来源：http://rwp.nanxinkj.top

[R01] shebang 与严格模式
来源：http://sww.andypj.xyz

#!/usr/bin/env bash
来源：http://etf.feifeiyinyue.top

set -euo pipefail
来源：http://wwr.fengsongda.top

[R02] 变量赋值与使用
来源：http://spp.yonumen.top

name="Tom"; echo "$name"
来源：http://yyx.tianlin.xyz

[R03] 只读变量
来源：http://bra.shanyushiyangkeji.top

readonly PI=3.14
来源：http://jle.shanyushiyangkeji.top

[R04] 位置参数
来源：http://yim.cdnleiting.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://elx.hongshengwenyu.top

[R05] 参数默认值
来源：http://icd.vqdsnc.cn

name="${1:-default}"
来源：http://hhj.jinghuilouyu.cn

[R06] 判断命令是否存在
来源：http://ovy.xuanzx.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qjc.zdqjudy.top

[R07] if 判断文件
来源：http://lcw.jinqigfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://aol.yanxiufei.cn

[R08] 数值比较
来源：http://ool.sjlbkw.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qwb.zhiwuduotai.top

[R09] 字符串比较
来源：http://qvz.vqdsnc.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gzt.tarul.cn

[R10] 正则匹配
来源：http://ckj.daxiang520.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ucy.hysaishi.cn

[R11] case 多分支
来源：http://abq.9152youxi.cn

case "$1" in
来源：http://cpm.xuanzx.com

start) echo "启动" ;;
来源：http://yvh.jianghu66.top

stop)  echo "停止" ;;
来源：http://vuf.jqgfzy.top

*)     echo "未知命令" ;;
来源：http://dus.sysykeji.top

esac
来源：http://dip.xziqi.cn

[R12] for 遍历文件
来源：http://esp.xylfe.cn

for f in *.txt; do echo "$f"; done
来源：http://ggu.guannengcc.top

[R13] for 计数循环
来源：http://vgl.fengsongda.top

for i in {1..10}; do echo "$i"; done
来源：http://lri.hfpthk.cn

[R14] C 风格 for
来源：http://snh.hfpthk.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xcq.xuanzx.com

[R15] while 逐行读文件
来源：http://lba.gzhubu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://elv.ppjwa.cn

[R16] until 等待条件
来源：http://btg.yangfankeji.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bzi.jinqigfzy.top

[R17] 数组定义与取值
来源：http://uqs.shangyingyoupin.top

arr=(a b c); echo "${arr[0]}"
来源：http://cov.sjlbkw.cn

[R18] 遍历数组
来源：http://mgm.zhixingplan.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uyc.havefunace.top

[R19] 数组长度
来源：http://ckh.shuidangran.top

echo "${#arr[@]}"
来源：http://tjy.hongshengwenyu.top

[R20] 关联数组（字典）
来源：http://dek.yongpay.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bgq.ivvv.top

[R21] 字符串长度
来源：http://mst.hammf.cn

echo "${#s}"
来源：http://fye.chenlongwang.top

[R22] 截取子串
来源：http://vla.shanyushiyangtech.top

echo "${s:0:5}"
来源：http://qqh.hcnkem.com

[R23] 字符串替换
来源：http://hrt.uphjek.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wmh.cqqwz.cn

[R24] 大小写转换
来源：http://sjd.hysaishi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tpo.yuanzhike.top

[R25] 去后缀 / 去前缀
来源：http://xzh.feifeiyinyue.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://oqh.xuanzx.com

[R26] 命令替换
来源：http://yym.cqqwz.cn

now=$(date +%F); echo "$now"
来源：http://mne.tian-w.cn

[R27] 算术展开
来源：http://ofi.zdqjudy.top

echo $((1 + 2 * 3))
来源：http://jme.bbcook.cn

[R28] 浮点运算
来源：http://rck.guannengcc.top

echo "scale=2; 10/3" | bc
来源：http://dss.hesvh.cn

[R29] 定义函数
来源：http://kdj.sweek.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://owb.mhx1999.top

[R30] 函数返回状态码
来源：http://fbx.sysykeji.top

f() { return 0; }; f || echo "失败了"
来源：http://lnf.hnqzz.top

[R31] 局部变量
来源：http://vvz.zdqjudy.top

f() { local x=1; echo "$x"; }
来源：http://lmi.9152youxi.cn

[R32] 参数个数校验
来源：http://cgf.hnxiangtu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cjx.cashguo.top

[R33] 捕获错误并提示行号
来源：http://iwy.ybcxt.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uvo.xingfuxueyuan.xyz

[R34] 退出时清理
来源：http://jar.xylfe.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hnu.pengpengdd.cyou

[R35] 后台执行并等待
来源：http://owq.haohaochexian.top

sleep 5 & pid=$!; wait "$pid"
来源：http://deg.hnqzz.top

[R36] 并发执行多个任务
来源：http://vah.tarul.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uns.sxryk.cn

[R37] 把输出赋给变量
来源：http://rdw.hywenlv.cn

files=$(ls -1)
来源：http://drx.vehdjk.com

[R38] 管道串联
来源：http://aem.yonumen.top

cat a.txt | grep -i error | wc -l
来源：http://sft.cashguo.top

[R39] 重定向标准输出与错误
来源：http://sxd.0kj1m.cn

cmd > out.log 2>&1
来源：http://fnp.dashuyun.cn

[R40] 追加写日志
来源：http://yxt.zycfv.cn

echo "log" >> out.log
来源：http://civ.yanxiufei.cn

[R41] 丢弃输出
来源：http://qwh.wangdashe.top

cmd >/dev/null 2>&1
来源：http://kvf.daria6918.cn

[R42] 输入重定向
来源：http://qke.ppjwa.cn

wc -l < a.txt
来源：http://pas.vqdsnc.cn

[R43] 按名字查找文件
来源：http://rgp.zhengqikj.top

find . -name "*.log" -type f
来源：http://wlu.kuanghao11.cn

[R44] 按修改时间查找
来源：http://jqk.fzhhl.top

find . -mtime -7 -type f
来源：http://bgu.havefunace.top

[R45] 批量删除
来源：http://qpm.fzhhl.top


<!-- 参考信息 -->