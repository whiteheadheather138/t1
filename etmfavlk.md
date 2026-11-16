代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://psi.fehbvm.com

user_id INT NOT NULL,
来源：http://qxt.iojbl.cn

amount DECIMAL(10, 2),
来源：http://spv.zhongyouzk.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zak.jinqigufen.top

);
来源：http://mrr.zhongyouzk.top

[Q03] 增加列
来源：http://lfm.ivvv.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://meu.xylfe.cn

[Q04] 修改列类型
来源：http://ksy.xziqi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://slq.uphjek.com

[Q05] 重命名列
来源：http://ter.hnqzz.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://itf.zhengqikj.top

[Q06] 删除列
来源：http://xvd.cucudq.cn

ALTER TABLE users DROP COLUMN age;
来源：http://skd.redwolf501.top

[Q07] 删除表
来源：http://nfu.pycfn.com

DROP TABLE IF EXISTS orders;
来源：http://uiz.zdbjq.cn

[Q08] 创建普通索引
来源：http://dis.jinqigfzy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://mka.kuanghao11.cn

[Q09] 创建唯一索引
来源：http://pjt.9152youxi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xby.birdmap.top

[Q10] 插入单行
来源：http://xri.hfpthk.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qps.tian-w.cn

[Q11] 一次插入多行
来源：http://ptf.chenlongwang.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pdy.gaohongyu789.top

[Q12] 插入后取自增 ID
来源：http://mcd.9152youxi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ftd.pycfn.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xxr.jyoumei.cn

[Q13] 忽略重复插入
来源：http://bld.ppjwa.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ohr.hywenlv.cn

[Q14] 存在则更新（upsert）
来源：http://orq.guowangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wqr.hywenlv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xrd.yj202588.top

[Q15] 查询全部
来源：http://wvx.zhongyouzk.top

SELECT * FROM users;
来源：http://xbl.hesvh.cn

[Q16] 查询指定列
来源：http://ntk.chenjidiqi.icu

SELECT id, name FROM users;
来源：http://gax.ydzc1.top

[Q17] 条件查询
来源：http://gml.jlsjyb.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://foa.ybcxt.top

[Q18] 模糊匹配
来源：http://ilj.fktsv.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://auj.316326.xyz

[Q19] 范围查询
来源：http://kng.meibo888.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tke.fehbvm.com

[Q20] IN 列表
来源：http://rmw.tanke756.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cmk.shanyushiyangkeji.top

[Q21] 空值判断
来源：http://ick.zhixingplan.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ocz.yanxiufei.cn

[Q22] 排序
来源：http://icr.wangdashe.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://oto.nanxinkj.top

[Q23] 分页
来源：http://pvj.shanyushiyangkeji.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sgw.iojbl.cn

[Q24] 去重
来源：http://lfp.yfazqb.com

SELECT DISTINCT city FROM users;
来源：http://ipi.cucudq.cn

[Q25] 只取前 N 条
来源：http://sbo.zhiwuduotai.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xur.fanxiaobao.xyz

[Q26] 计数
来源：http://dtc.mhx1999.top

SELECT COUNT(*) FROM users;
来源：http://jzk.vqdsnc.cn

[Q27] 条件计数
来源：http://znk.zhongyouzk.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ecd.shanyushiyangtech.top

[Q28] 求和与平均
来源：http://rfy.fanxiaobao.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sdt.yuanzhike.top

[Q29] 最大最小值
来源：http://oew.zhengqikj.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jex.hnxiangtu.top

[Q30] 分组统计
来源：http://uqf.yangfankeji.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://aqo.hnxiangtu.top

[Q31] 分组后过滤
来源：http://dsf.jyoumei.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nao.yvedp.cn

[Q32] 分组拼接字符串
来源：http://cgm.yvedp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ejb.shangyingyoupin.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yhi.hcnkem.com

[Q33] 多列分组
来源：http://wvw.52xcode.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xbu.pycfn.com

[Q34] 每组取第一条
来源：http://xhn.yongpay.top

SELECT * FROM (
来源：http://iod.chenzaomai.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://amb.chenzaomai.com

) t WHERE rn = 1;
来源：http://ryf.vehdjk.com

[Q35] 内连接
来源：http://fnd.vehdjk.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ikl.zhoulong.xyz

[Q36] 左连接
来源：http://dyh.nanxuanxn.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dvb.cdnleiting.top

[Q37] 右连接
来源：http://ele.xylfe.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jmn.haohaochexian.top

[Q38] 全外连接（PostgreSQL）
来源：http://lju.vqdsnc.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rle.sweek.top

[Q39] 自连接（查上下级）
来源：http://cfd.zdqjudy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://dvn.zhoulong.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tmi.hesvh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mll.xuetiantiany.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xre.uphjek.com

[Q41] 多表连接
来源：http://ysv.yanxiufei.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fev.cheryme.top

JOIN users u ON u.id = o.user_id
来源：http://hos.zhijiandao.cn

JOIN products p ON p.id = o.product_id;
来源：http://kyt.shanyushiyangkeji.top

[Q42] 连接条件附加过滤
来源：http://cpo.xuetiantiany.cn

SELECT u.name, o.amount FROM users u
来源：http://okg.chenzaomai.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hhm.hysaishi.cn

[Q43] 标量子查询
来源：http://aly.sjlbkw.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jcy.dashuyun.cn

[Q44] IN 子查询
来源：http://amy.zdqjudy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sun.tarul.cn

[Q45] EXISTS 判断存在
来源：http://ltr.shanyushiyangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nla.tian-w.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vnf.fktsv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ruy.fengsongda.top

[Q47] 与平均值比较
来源：http://uti.ywan-chungtsiang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://iar.sjlbkw.cn

[Q48] CTE 公用表表达式
来源：http://isc.gotoacloud.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hvr.havefunace.top

SELECT * FROM t WHERE c > 5;
来源：http://ris.yangfankeji.com

[Q49] 更新单行
来源：http://xys.yj20258.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pfq.shzxlz.cn

[Q50] 批量更新
来源：http://rdz.quarkkingdee.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wqe.ivvv.top

[Q51] 用子查询更新
来源：http://pza.jqgufenzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oge.hysaishi.cn

[Q52] 删除指定行
来源：http://fzi.hfpthk.cn

DELETE FROM users WHERE id = 10;
来源：http://xyc.zdbjq.cn

[Q53] 按条件删除
来源：http://jqm.daxiang520.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ntn.ctjpmb.com

[Q54] 清空表
来源：http://pfh.feifeiyinyue.top

TRUNCATE TABLE logs;
来源：http://sne.ybcxt.top

[Q55] 排名（并列占位）
来源：http://rbm.xylfe.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dnx.316326.xyz

[Q56] 密集排名（并列不占位）
来源：http://mrj.cashguo.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ava.zhengqikj.top

[Q57] 行号
来源：http://ltp.redwolf501.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nyg.ivvv.top

[Q58] 累计求和
来源：http://mwz.nanxinkj.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fep.gzhubu.top

[Q59] 分组内累计
来源：http://bom.zhijiandao.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nmb.shzxlz.cn

[Q60] 取上一行 / 下一行
来源：http://omn.yj20258888.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uqw.0kj1m.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xvt.zhaomingkeji.xyz

[Q61] 移动平均
来源：http://mfz.ydjk.org.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pps.chenlongwang.top

[Q62] 分组占比
来源：http://jfb.jyoumei.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dtb.cucudq.cn

[Q63] 开启事务
来源：http://dli.jianghu66.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jsq.yj202588.top

[Q64] 提交事务
来源：http://udr.feifeiyinyue.top

COMMIT;
来源：http://fat.jyoumei.cn

[Q65] 回滚事务
来源：http://vuc.hcnkem.com

ROLLBACK;
来源：http://dqh.ydzc1.top

[Q66] 行锁查询
来源：http://mir.daxiang520.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rfl.jianghu66.top

[Q67] 设置隔离级别
来源：http://qgo.jianghu66.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oho.zhaomingkeji.xyz

[Q68] 保存点
来源：http://kzo.tian-w.cn

SAVEPOINT sp1;
来源：http://vdj.dianchejie.cn

ROLLBACK TO sp1;
来源：http://bxb.ppjwa.cn

[Q69] 查看执行计划
来源：http://huz.52xcode.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lqz.daxiang520.top

[Q70] 更新统计信息
来源：http://jhp.shanyushiyangkeji.top

ANALYZE TABLE users;
来源：http://mje.jqgufenzy.top

[Q71] 查看建表语句
来源：http://czs.hcnkem.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ewc.mhx1999.top

[Q72] 查看索引
来源：http://zse.zhijiandao.cn

SHOW INDEX FROM users;
来源：http://xfm.fzhhl.top

[Q73] 查看表状态
来源：http://jcz.guannengcc.top

SHOW TABLE STATUS LIKE 'users';
来源：http://elx.yongpay.top

[Q74] 强制使用索引
来源：http://qbn.hammf.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://usk.yj20258.top

[Q75] 日期格式化
来源：http://iuq.jianghu66.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zyp.ehwqpu.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ghl.zhiwuduotai.top

[Q76] 按天统计
来源：http://jvn.cqqwz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ahr.meibo888.top

[Q77] 时间加减
来源：http://zmb.zhengqikj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wws.nanxuanxn.top

[Q78] 当前时间
来源：http://qop.tianlin.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oin.jyoumei.cn

[Q79] 字符串拼接
来源：http://npt.fzhhl.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qvy.zycfv.cn

[Q80] 字符串截取
来源：http://rbw.c1oappe.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mjg.shuidangran.top

[Q81] 字符串替换
来源：http://rcn.zdbjq.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lqm.fzhhl.top

[Q82] 字符长度与字节长度
来源：http://luj.yj20258.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nmf.316326.xyz

[Q83] 大小写转换
来源：http://ftw.haohaochexian.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wln.wangdashe.top

[Q84] 去除首尾空格
来源：http://brz.aibaodan.cn

SELECT TRIM(name) FROM users;
来源：http://fbp.epnwcf.com

[Q85] 数值取整
来源：http://arh.jinqigufen.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bwf.yonumen.top

[Q86] 读取 JSON 字段
来源：http://htj.hfpthk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ljy.ctjpmb.com

[Q87] JSON 字段做条件
来源：http://gzf.bjfxy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xds.gotoacloud.top

[Q88] 行转列（条件聚合）
来源：http://dlt.gaohongyu789.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wgj.ydjk.org.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jlu.tian-w.cn

[Q89] 判断表是否存在
来源：http://svg.jlsjyb.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bwj.316326.xyz

[Q90] 生成序号列
来源：http://sos.wangshuangyany.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jas.yvedp.cn

================================================================================
来源：http://zwd.pycfn.com

R. Bash 专题
来源：http://iby.ehwqpu.com

================================================================================
来源：http://gzk.zhengqikj.top

[R01] shebang 与严格模式
来源：http://xxm.xingfuxueyuan.xyz

#!/usr/bin/env bash
来源：http://nhk.wangdashe.top

set -euo pipefail
来源：http://sgo.sysykeji.top

[R02] 变量赋值与使用
来源：http://shi.guannengcc.top

name="Tom"; echo "$name"
来源：http://okx.iojbl.cn

[R03] 只读变量
来源：http://qkq.nwbrower.top

readonly PI=3.14
来源：http://ztc.wangdashe.top

[R04] 位置参数
来源：http://rgf.cqqwz.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lot.cqqwz.cn

[R05] 参数默认值
来源：http://yzj.pycfn.com

name="${1:-default}"
来源：http://kzh.316326.xyz

[R06] 判断命令是否存在
来源：http://xhy.gzhubu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jiq.smart0.xyz

[R07] if 判断文件
来源：http://nbn.andypj.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uts.cdnleiting.top

[R08] 数值比较
来源：http://rxi.jinghuilouyu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mda.sweek.top

[R09] 字符串比较
来源：http://vgw.cheryme.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zyu.cucudq.cn

[R10] 正则匹配
来源：http://tff.shzxlz.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://olf.hfpthk.cn

[R11] case 多分支
来源：http://hor.cheryme.top

case "$1" in
来源：http://cls.hnqzz.top

start) echo "启动" ;;
来源：http://cay.jlsjyb.cn

stop)  echo "停止" ;;
来源：http://mmi.uphjek.com

*)     echo "未知命令" ;;
来源：http://biy.wangshuangyany.cn

esac
来源：http://fjn.zhengqikj.top

[R12] for 遍历文件
来源：http://bpm.jinqigufen.top

for f in *.txt; do echo "$f"; done
来源：http://uvk.snrcjt.cn

[R13] for 计数循环
来源：http://enl.yangfankeji.com

for i in {1..10}; do echo "$i"; done
来源：http://mbf.nwbrower.top

[R14] C 风格 for
来源：http://afb.jinyuanbaomall.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hhd.guowangkeji.top

[R15] while 逐行读文件
来源：http://hdv.pycfn.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://smy.ywan-chungtsiang.top

[R16] until 等待条件
来源：http://yhs.feifeiyinyue.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dgs.wangshuangyany.cn

[R17] 数组定义与取值
来源：http://yuy.zdbjq.cn

arr=(a b c); echo "${arr[0]}"
来源：http://egq.xylfe.cn

[R18] 遍历数组
来源：http://quz.shuidangran.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dhp.xingfuxueyuan.xyz

[R19] 数组长度
来源：http://nhb.svipenyu.cn

echo "${#arr[@]}"
来源：http://mlw.zdqjudy.top

[R20] 关联数组（字典）
来源：http://utw.shanyushiyangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ymn.aibaodan.cn

[R21] 字符串长度
来源：http://inr.jinqigfzy.top

echo "${#s}"
来源：http://jfe.quarkkingdee.top

[R22] 截取子串
来源：http://nye.jinqigufen.top

echo "${s:0:5}"
来源：http://mje.jlsjyb.cn

[R23] 字符串替换
来源：http://aeo.guannengcc.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rdu.vqdsnc.cn

[R24] 大小写转换
来源：http://hek.wangdashe.top

echo "${s^^}"; echo "${s,,}"
来源：http://hoo.quarkkingdee.top

[R25] 去后缀 / 去前缀
来源：http://nlp.9152youxi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pci.c1oappe.top

[R26] 命令替换
来源：http://uea.daria6918.cn

now=$(date +%F); echo "$now"
来源：http://sdn.jinyuanbaomall.cn

[R27] 算术展开
来源：http://umn.aizwys.cn

echo $((1 + 2 * 3))
来源：http://utu.guowangkeji.top

[R28] 浮点运算
来源：http://iqj.sweek.top

echo "scale=2; 10/3" | bc
来源：http://rhn.xuetiantiany.cn

[R29] 定义函数
来源：http://wnl.jqgufenzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hwb.hywenlv.cn

[R30] 函数返回状态码
来源：http://fvt.fzhhl.top

f() { return 0; }; f || echo "失败了"
来源：http://mqj.haohaochexian.top

[R31] 局部变量
来源：http://kxx.jinyuanbaomall.cn

f() { local x=1; echo "$x"; }
来源：http://lmo.sxryk.cn

[R32] 参数个数校验
来源：http://uea.jqgufenzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yck.dashuyun.cn

[R33] 捕获错误并提示行号
来源：http://sty.hcnkem.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gmk.nanxuanxn.top

[R34] 退出时清理
来源：http://brg.xinyue.icu

trap 'rm -f "$tmp"' EXIT
来源：http://uzl.fanxiaobao.xyz

[R35] 后台执行并等待
来源：http://ftx.yj20258888.top

sleep 5 & pid=$!; wait "$pid"
来源：http://vgc.52xcode.cn

[R36] 并发执行多个任务
来源：http://iua.shzxlz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://njo.sysykeji.top

[R37] 把输出赋给变量
来源：http://nsp.316326.xyz

files=$(ls -1)
来源：http://xws.yanxiufei.cn

[R38] 管道串联
来源：http://yep.aibaodan.cn

cat a.txt | grep -i error | wc -l
来源：http://peg.gogol.net.cn

[R39] 重定向标准输出与错误
来源：http://heq.chenjidiqi.icu

cmd > out.log 2>&1
来源：http://rpe.wangdashe.top

[R40] 追加写日志
来源：http://bct.bbcook.cn

echo "log" >> out.log
来源：http://jbh.zhongyouzk.top

[R41] 丢弃输出
来源：http://tgq.havefunace.top

cmd >/dev/null 2>&1
来源：http://sdq.redwolf501.top

[R42] 输入重定向
来源：http://adu.xuanzx.com

wc -l < a.txt
来源：http://lov.c1oappe.top

[R43] 按名字查找文件
来源：http://dht.gzhubu.top

find . -name "*.log" -type f
来源：http://gpv.yfazqb.com

[R44] 按修改时间查找
来源：http://npq.xylfe.cn

find . -mtime -7 -type f
来源：http://cgn.gaohongyu789.top

[R45] 批量删除
来源：http://tda.ybcxt.top

find . -name "*.tmp" -delete
来源：http://idp.fktsv.cn

[R46] 递归替换文件内容
来源：http://ybi.nwbrower.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uxk.xylfe.cn

[R47] sed 单行替换
来源：http://pcy.yfazqb.com

sed -i 's/foo/bar/g' a.txt
来源：http://jsv.hfpthk.cn

[R48] awk 取指定列
来源：http://qwg.smart0.xyz

awk '{print $1, $3}' a.txt
来源：http://uts.jinqigfzy.top

[R49] awk 带条件
来源：http://rkg.birdmap.top


<!-- 参考信息 -->