代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vbb.zdqjudy.top

);
来源：http://kiw.yuanzhike.top

[Q02] 创建带外键的表
来源：http://eva.ydzc1.top

CREATE TABLE orders (
来源：http://tpu.redwolf501.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kdi.fktsv.cn

user_id INT NOT NULL,
来源：http://rnv.hongshengwenyu.top

amount DECIMAL(10, 2),
来源：http://auf.dashuyun.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ltp.kuanghao11.cn

);
来源：http://cob.dashuyun.cn

[Q03] 增加列
来源：http://nvs.shzxlz.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dnu.fehbvm.com

[Q04] 修改列类型
来源：http://ybk.tianlin.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cmk.zhongyouzk.top

[Q05] 重命名列
来源：http://drj.yangfankeji.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://urh.yuxming.cn

[Q06] 删除列
来源：http://fob.zhiwuduotai.top

ALTER TABLE users DROP COLUMN age;
来源：http://erq.xinyue.icu

[Q07] 删除表
来源：http://qft.316326.xyz

DROP TABLE IF EXISTS orders;
来源：http://lxo.zhijiandao.cn

[Q08] 创建普通索引
来源：http://pzr.cheryme.top

CREATE INDEX idx_users_email ON users(email);
来源：http://hhc.sxryk.cn

[Q09] 创建唯一索引
来源：http://ofu.fehbvm.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bjx.shanyushiyangtech.top

[Q10] 插入单行
来源：http://ygy.hongshengwenyu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cka.shanyushiyangtech.top

[Q11] 一次插入多行
来源：http://isa.yonumen.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ikl.sjlbkw.cn

[Q12] 插入后取自增 ID
来源：http://bvo.nwbrower.top

INSERT INTO users (name) VALUES ('C');
来源：http://psc.xingfuxueyuan.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qqp.c1oappe.top

[Q13] 忽略重复插入
来源：http://nku.cucudq.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hlv.yvedp.cn

[Q14] 存在则更新（upsert）
来源：http://xyc.xinyue.icu

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nbs.yfazqb.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jnz.jinqigfzy.top

[Q15] 查询全部
来源：http://nsl.zdqjudy.top

SELECT * FROM users;
来源：http://jtc.snrcjt.cn

[Q16] 查询指定列
来源：http://gqx.gzhubu.top

SELECT id, name FROM users;
来源：http://zpy.jlsjyb.cn

[Q17] 条件查询
来源：http://aiy.hnqzz.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ijh.meibo888.top

[Q18] 模糊匹配
来源：http://tix.feifeiyinyue.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dyv.yj202588.top

[Q19] 范围查询
来源：http://gss.pengpengdd.cyou

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://prd.cdnleiting.top

[Q20] IN 列表
来源：http://lov.yfazqb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gne.tianlin.xyz

[Q21] 空值判断
来源：http://qam.hysaishi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://oxf.hywenlv.cn

[Q22] 排序
来源：http://boe.sweek.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gha.yj202588.top

[Q23] 分页
来源：http://ryf.0kj1m.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rsa.dashuyun.cn

[Q24] 去重
来源：http://eiq.shanyushiyangkeji.top

SELECT DISTINCT city FROM users;
来源：http://cku.fzhhl.top

[Q25] 只取前 N 条
来源：http://fpu.cqqwz.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dho.fehbvm.com

[Q26] 计数
来源：http://jyh.jlsjyb.cn

SELECT COUNT(*) FROM users;
来源：http://hxu.mhx1999.top

[Q27] 条件计数
来源：http://hzj.shuidangran.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vdi.yanxiufei.cn

[Q28] 求和与平均
来源：http://ujz.zhijiandao.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uas.xylfe.cn

[Q29] 最大最小值
来源：http://eso.hongshengwenyu.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://dfs.zdqjudy.top

[Q30] 分组统计
来源：http://twy.gotoacloud.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qem.jinghuilouyu.cn

[Q31] 分组后过滤
来源：http://dxl.jqgfzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qtw.cdnleiting.top

[Q32] 分组拼接字符串
来源：http://sky.jqgfzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://isf.nanxinkj.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lvy.smart0.xyz

[Q33] 多列分组
来源：http://bym.ppjwa.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ght.iojbl.cn

[Q34] 每组取第一条
来源：http://ccx.vqdsnc.cn

SELECT * FROM (
来源：http://aqh.fengsongda.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kud.aibaodan.cn

) t WHERE rn = 1;
来源：http://lvk.chenjidiqi.icu

[Q35] 内连接
来源：http://bff.cqqwz.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ydn.hnxiangtu.top

[Q36] 左连接
来源：http://une.ydzc1.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gmf.yongpay.top

[Q37] 右连接
来源：http://fbn.316326.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lvx.9152youxi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ija.wangshuangyany.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vhs.gaohongyu789.top

[Q39] 自连接（查上下级）
来源：http://hqv.sjlbkw.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wbh.316326.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://izc.nwbrower.top

[Q40] 交叉连接（笛卡尔积）
来源：http://nmf.epnwcf.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ndy.zycfv.cn

[Q41] 多表连接
来源：http://tlf.sufxvd.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gaw.cdnleiting.top

JOIN users u ON u.id = o.user_id
来源：http://itu.chenlongwang.top

JOIN products p ON p.id = o.product_id;
来源：http://ugw.shanyushiyangkeji.top

[Q42] 连接条件附加过滤
来源：http://ghm.tianlin.xyz

SELECT u.name, o.amount FROM users u
来源：http://zwn.sxryk.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zcj.dianchejie.cn

[Q43] 标量子查询
来源：http://hev.tian-w.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ili.svipenyu.cn

[Q44] IN 子查询
来源：http://mzx.jiagoushi.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://spd.xinyue.icu

[Q45] EXISTS 判断存在
来源：http://ooe.shzxlz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://geu.bjfxy.top

[Q46] NOT EXISTS 判断不存在
来源：http://xgk.andypj.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hbd.cdnleiting.top

[Q47] 与平均值比较
来源：http://qgf.tian-w.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cmf.52xcode.cn

[Q48] CTE 公用表表达式
来源：http://xrx.sxryk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xtn.yvedp.cn

SELECT * FROM t WHERE c > 5;
来源：http://evs.yanxiufei.cn

[Q49] 更新单行
来源：http://bpg.chenzaomai.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://opu.yongpay.top

[Q50] 批量更新
来源：http://vgt.hywenlv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zyn.0kj1m.cn

[Q51] 用子查询更新
来源：http://chi.gzhubu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cbw.pycfn.com

[Q52] 删除指定行
来源：http://avu.shangyingyoupin.top

DELETE FROM users WHERE id = 10;
来源：http://mha.jlsjyb.cn

[Q53] 按条件删除
来源：http://xlj.xuanzx.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mqr.zhaomingkeji.xyz

[Q54] 清空表
来源：http://var.yanxiufei.cn

TRUNCATE TABLE logs;
来源：http://vaz.52xcode.cn

[Q55] 排名（并列占位）
来源：http://ofr.xziqi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xtl.wangshuangyany.cn

[Q56] 密集排名（并列不占位）
来源：http://kbj.zdqjudy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dxq.kuanghao11.cn

[Q57] 行号
来源：http://cpj.vqdsnc.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xrz.cheryme.top

[Q58] 累计求和
来源：http://ysz.jianghu66.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://obb.jyoumei.cn

[Q59] 分组内累计
来源：http://scj.vehdjk.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jzl.cheryme.top

[Q60] 取上一行 / 下一行
来源：http://wmi.ctjpmb.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kuy.jinyuanbaomall.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ixn.cheryme.top

[Q61] 移动平均
来源：http://ekl.gogol.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vvu.hywenlv.cn

[Q62] 分组占比
来源：http://ezz.wangdashe.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cec.sweek.top

[Q63] 开启事务
来源：http://xny.vehdjk.com

START TRANSACTION;                -- 或 BEGIN
来源：http://ugh.xziqi.cn

[Q64] 提交事务
来源：http://txx.zdbjq.cn

COMMIT;
来源：http://xmo.havefunace.top

[Q65] 回滚事务
来源：http://plg.xuetiantiany.cn

ROLLBACK;
来源：http://cxy.zhengqikj.top

[Q66] 行锁查询
来源：http://yek.xziqi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://exy.zhengqikj.top

[Q67] 设置隔离级别
来源：http://gbf.fengsongda.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ylo.sxryk.cn

[Q68] 保存点
来源：http://wvh.aizwys.cn

SAVEPOINT sp1;
来源：http://bxu.xziqi.cn

ROLLBACK TO sp1;
来源：http://ggb.yuxming.cn

[Q69] 查看执行计划
来源：http://keb.vqdsnc.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jev.nanxuanxn.top

[Q70] 更新统计信息
来源：http://pta.ppjwa.cn

ANALYZE TABLE users;
来源：http://gam.jinqigfzy.top

[Q71] 查看建表语句
来源：http://hna.yuxming.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dlf.ydzc1.top

[Q72] 查看索引
来源：http://isk.c1oappe.top

SHOW INDEX FROM users;
来源：http://hmv.fengsongda.top

[Q73] 查看表状态
来源：http://zzk.ydjk.org.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cia.zhoulong.xyz

[Q74] 强制使用索引
来源：http://ijv.shuidangran.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://urd.havefunace.top

[Q75] 日期格式化
来源：http://bgo.hcnkem.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://flz.sjlbkw.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hjd.fanxiaobao.xyz

[Q76] 按天统计
来源：http://hsc.guannengcc.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vas.aibaodan.cn

[Q77] 时间加减
来源：http://kdf.fzhhl.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ihi.xylfe.cn

[Q78] 当前时间
来源：http://qmq.svipenyu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://isr.ehwqpu.com

[Q79] 字符串拼接
来源：http://bvl.316326.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jqa.yj20258888.top

[Q80] 字符串截取
来源：http://wmy.hongshengwenyu.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lad.0kj1m.cn

[Q81] 字符串替换
来源：http://drk.feifeiyinyue.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fvp.pengpengdd.cyou

[Q82] 字符长度与字节长度
来源：http://wir.havefunace.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tst.hysaishi.cn

[Q83] 大小写转换
来源：http://iee.zhijiandao.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kmx.andypj.xyz

[Q84] 去除首尾空格
来源：http://ytx.jqgufenzy.top

SELECT TRIM(name) FROM users;
来源：http://gsc.guowangkeji.top

[Q85] 数值取整
来源：http://kha.havefunace.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rbv.zycfv.cn

[Q86] 读取 JSON 字段
来源：http://idy.jqgufenzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cqd.xylfe.cn

[Q87] JSON 字段做条件
来源：http://fsc.feifeiyinyue.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://una.ehwqpu.com

[Q88] 行转列（条件聚合）
来源：http://pzg.sxryk.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jjb.zhengqikj.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fkq.chenlongwang.top

[Q89] 判断表是否存在
来源：http://cxc.zhijiandao.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mkk.yj20258.top

[Q90] 生成序号列
来源：http://xbk.jinqigufen.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yjp.sxryk.cn

================================================================================
来源：http://ose.aizwys.cn

R. Bash 专题
来源：http://ojq.vqdsnc.cn

================================================================================
来源：http://rtd.mhx1999.top

[R01] shebang 与严格模式
来源：http://yuy.bbcook.cn

#!/usr/bin/env bash
来源：http://rzt.316326.xyz

set -euo pipefail
来源：http://wao.fanxiaobao.xyz

[R02] 变量赋值与使用
来源：http://fvo.bjfxy.top

name="Tom"; echo "$name"
来源：http://ybs.ywan-chungtsiang.top

[R03] 只读变量
来源：http://sso.hesvh.cn

readonly PI=3.14
来源：http://ola.fehbvm.com

[R04] 位置参数
来源：http://ipe.yueranfly.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://enn.cdnleiting.top

[R05] 参数默认值
来源：http://jpr.jqgufenzy.top

name="${1:-default}"
来源：http://paw.zhongyouzk.top

[R06] 判断命令是否存在
来源：http://bks.52xcode.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pxu.hongshengwenyu.top

[R07] if 判断文件
来源：http://rvg.tarul.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bph.hammf.cn

[R08] 数值比较
来源：http://vcp.nanxuanxn.top

if (( a > b )); then echo "a 更大"; fi
来源：http://tsm.aizwys.cn

[R09] 字符串比较
来源：http://hxr.yuxming.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://iju.mhx1999.top

[R10] 正则匹配
来源：http://ign.nanxuanxn.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ahr.hongshengwenyu.top

[R11] case 多分支
来源：http://bdm.xuetiantiany.cn

case "$1" in
来源：http://vat.nanxinkj.top

start) echo "启动" ;;
来源：http://rwo.chenjidiqi.icu

stop)  echo "停止" ;;
来源：http://uzq.tian-w.cn

*)     echo "未知命令" ;;
来源：http://yzg.shanyushiyangtech.top

esac
来源：http://vdq.vehdjk.com

[R12] for 遍历文件
来源：http://nes.yfazqb.com

for f in *.txt; do echo "$f"; done
来源：http://obs.c1oappe.top

[R13] for 计数循环
来源：http://xrb.zycfv.cn

for i in {1..10}; do echo "$i"; done
来源：http://onf.fanxiaobao.xyz

[R14] C 风格 for
来源：http://uxd.hfpthk.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://toy.ydjk.org.cn

[R15] while 逐行读文件
来源：http://jcz.chenjidiqi.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ynj.nwbrower.top

[R16] until 等待条件
来源：http://jow.quarkkingdee.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hsr.fehbvm.com

[R17] 数组定义与取值
来源：http://lni.ybcxt.top

arr=(a b c); echo "${arr[0]}"
来源：http://hkb.feifeiyinyue.top

[R18] 遍历数组
来源：http://hsc.9152youxi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pka.shanyushiyangkeji.top

[R19] 数组长度
来源：http://taw.epnwcf.com

echo "${#arr[@]}"
来源：http://wfu.jinyuanbaomall.cn

[R20] 关联数组（字典）
来源：http://phk.svipenyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://roh.ydzc1.top

[R21] 字符串长度
来源：http://xzb.chenjidiqi.icu

echo "${#s}"
来源：http://moj.hnqzz.top

[R22] 截取子串
来源：http://pgs.epnwcf.com

echo "${s:0:5}"
来源：http://ytw.yueranfly.top

[R23] 字符串替换
来源：http://xyc.hywenlv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qcl.yanxiufei.cn

[R24] 大小写转换
来源：http://nml.jinghuilouyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nie.sjlbkw.cn

[R25] 去后缀 / 去前缀
来源：http://ovo.feifeiyinyue.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dla.mhx1999.top

[R26] 命令替换
来源：http://jhw.yonumen.top

now=$(date +%F); echo "$now"
来源：http://gvo.bjfxy.top

[R27] 算术展开
来源：http://kmh.xuanzx.com

echo $((1 + 2 * 3))
来源：http://wql.hnxiangtu.top

[R28] 浮点运算
来源：http://zur.yangfankeji.com

echo "scale=2; 10/3" | bc
来源：http://yan.gogol.net.cn

[R29] 定义函数
来源：http://fst.jyoumei.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ndg.hesvh.cn

[R30] 函数返回状态码
来源：http://siq.sxryk.cn

f() { return 0; }; f || echo "失败了"
来源：http://onn.chenlongwang.top

[R31] 局部变量
来源：http://afl.hywenlv.cn

f() { local x=1; echo "$x"; }
来源：http://cfv.cucudq.cn

[R32] 参数个数校验
来源：http://amo.xylfe.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cpk.ybcxt.top

[R33] 捕获错误并提示行号
来源：http://umn.ybcxt.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qcr.nanxinkj.top

[R34] 退出时清理
来源：http://ikd.yuanzhike.top

trap 'rm -f "$tmp"' EXIT
来源：http://mjn.tarul.cn

[R35] 后台执行并等待
来源：http://kmh.zhixingplan.top

sleep 5 & pid=$!; wait "$pid"
来源：http://rcf.jianghu66.top

[R36] 并发执行多个任务
来源：http://rpo.sufxvd.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ipd.wangdashe.top

[R37] 把输出赋给变量
来源：http://ntj.chenzaomai.com

files=$(ls -1)
来源：http://gts.aizwys.cn

[R38] 管道串联
来源：http://xfw.jianghu66.top

cat a.txt | grep -i error | wc -l
来源：http://zgz.hfpthk.cn

[R39] 重定向标准输出与错误
来源：http://kuu.zhaomingkeji.xyz

cmd > out.log 2>&1
来源：http://ylz.shuidangran.top

[R40] 追加写日志
来源：http://kvc.zhoulong.xyz

echo "log" >> out.log
来源：http://taa.c1oappe.top

[R41] 丢弃输出
来源：http://yny.shanyushiyangtech.top

cmd >/dev/null 2>&1
来源：http://xmx.yanxiufei.cn

[R42] 输入重定向
来源：http://ghi.shangyingyoupin.top

wc -l < a.txt
来源：http://fwt.ppjwa.cn

[R43] 按名字查找文件
来源：http://mxs.gogol.net.cn

find . -name "*.log" -type f
来源：http://rmx.dianchejie.cn

[R44] 按修改时间查找
来源：http://vck.xinyue.icu

find . -mtime -7 -type f
来源：http://ltz.yvedp.cn

[R45] 批量删除
来源：http://ioc.aizwys.cn

find . -name "*.tmp" -delete
来源：http://crh.hnqzz.top

[R46] 递归替换文件内容
来源：http://izh.quarkkingdee.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vlb.aibaodan.cn

[R47] sed 单行替换
来源：http://kiw.cdnleiting.top


<!-- 参考信息 -->