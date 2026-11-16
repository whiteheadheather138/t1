代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://vwq.guowangkeji.top

[Q09] 创建唯一索引
来源：http://qpo.bbcook.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ykq.gzhubu.top

[Q10] 插入单行
来源：http://gkr.hnxiangtu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jgu.0kj1m.cn

[Q11] 一次插入多行
来源：http://law.fzhhl.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jwt.ctjpmb.com

[Q12] 插入后取自增 ID
来源：http://vsw.ydjk.org.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cst.havefunace.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vhs.zhijiandao.cn

[Q13] 忽略重复插入
来源：http://snc.dianchejie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://akz.kuanghao11.cn

[Q14] 存在则更新（upsert）
来源：http://sjn.quarkkingdee.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cma.fengsongda.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bya.yongpay.top

[Q15] 查询全部
来源：http://jdp.fengsongda.top

SELECT * FROM users;
来源：http://gwy.nanxuanxn.top

[Q16] 查询指定列
来源：http://bts.jlsjyb.cn

SELECT id, name FROM users;
来源：http://que.yfazqb.com

[Q17] 条件查询
来源：http://mob.cheryme.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kzl.jlsjyb.cn

[Q18] 模糊匹配
来源：http://vkj.kuanghao11.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zhe.hesvh.cn

[Q19] 范围查询
来源：http://rcc.fanxiaobao.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vrz.aibaodan.cn

[Q20] IN 列表
来源：http://pgh.guowangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://edr.zhoulong.xyz

[Q21] 空值判断
来源：http://sre.jqgufenzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://vtr.xinyue.icu

[Q22] 排序
来源：http://nlq.fktsv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zlr.hnqzz.top

[Q23] 分页
来源：http://uvy.hfpthk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kwf.sjlbkw.cn

[Q24] 去重
来源：http://xjl.fzhhl.top

SELECT DISTINCT city FROM users;
来源：http://kmn.zhongyouzk.top

[Q25] 只取前 N 条
来源：http://yuu.ydzc1.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rck.yangfankeji.com

[Q26] 计数
来源：http://ggz.haohaochexian.top

SELECT COUNT(*) FROM users;
来源：http://usx.yongpay.top

[Q27] 条件计数
来源：http://olk.zhongyouzk.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xyp.zhongyouzk.top

[Q28] 求和与平均
来源：http://znk.zhiwuduotai.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jzj.cdnleiting.top

[Q29] 最大最小值
来源：http://ecw.jianghu66.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://pnk.ydzc1.top

[Q30] 分组统计
来源：http://vgw.pengpengdd.cyou

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wkm.guannengcc.top

[Q31] 分组后过滤
来源：http://taw.yuxming.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qyn.zdqjudy.top

[Q32] 分组拼接字符串
来源：http://usy.jlsjyb.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uie.chenlongwang.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uex.zhengqikj.top

[Q33] 多列分组
来源：http://xum.iojbl.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ofp.bjfxy.top

[Q34] 每组取第一条
来源：http://rkc.guowangkeji.top

SELECT * FROM (
来源：http://prh.cheryme.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gdu.vqdsnc.cn

) t WHERE rn = 1;
来源：http://ixd.cqqwz.cn

[Q35] 内连接
来源：http://ppp.hywenlv.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lhq.ehwqpu.com

[Q36] 左连接
来源：http://qkd.sjlbkw.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rve.chenjidiqi.icu

[Q37] 右连接
来源：http://gxe.zhoulong.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://myq.haohaochexian.top

[Q38] 全外连接（PostgreSQL）
来源：http://kfd.hesvh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ajz.c1oappe.top

[Q39] 自连接（查上下级）
来源：http://bjs.gogol.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://atg.yvedp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gyk.havefunace.top

[Q40] 交叉连接（笛卡尔积）
来源：http://nhx.tianlin.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dxx.haohaochexian.top

[Q41] 多表连接
来源：http://hnd.hongshengwenyu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bqw.aibaodan.cn

JOIN users u ON u.id = o.user_id
来源：http://vbz.xingfuxueyuan.xyz

JOIN products p ON p.id = o.product_id;
来源：http://duu.fktsv.cn

[Q42] 连接条件附加过滤
来源：http://ryf.guannengcc.top

SELECT u.name, o.amount FROM users u
来源：http://hwu.hcnkem.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pkk.9152youxi.cn

[Q43] 标量子查询
来源：http://sns.svipenyu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fcp.cdnleiting.top

[Q44] IN 子查询
来源：http://jdx.jinqigufen.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gdu.jinyuanbaomall.cn

[Q45] EXISTS 判断存在
来源：http://fxz.vehdjk.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yvq.dianchejie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nkp.yj202588.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kaa.sjlbkw.cn

[Q47] 与平均值比较
来源：http://avc.pycfn.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cnr.yanxiufei.cn

[Q48] CTE 公用表表达式
来源：http://hkb.pycfn.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fpr.zdqjudy.top

SELECT * FROM t WHERE c > 5;
来源：http://eim.jqgufenzy.top

[Q49] 更新单行
来源：http://alo.bbcook.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tdw.bbcook.cn

[Q50] 批量更新
来源：http://pdj.ybcxt.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oyq.yuxming.cn

[Q51] 用子查询更新
来源：http://hha.fehbvm.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cux.sweek.top

[Q52] 删除指定行
来源：http://gcv.guowangkeji.top

DELETE FROM users WHERE id = 10;
来源：http://bqf.nwbrower.top

[Q53] 按条件删除
来源：http://leb.gzhubu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rxz.zdqjudy.top

[Q54] 清空表
来源：http://kqz.zhongyouzk.top

TRUNCATE TABLE logs;
来源：http://tii.ctjpmb.com

[Q55] 排名（并列占位）
来源：http://bmc.aibaodan.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pie.cheryme.top

[Q56] 密集排名（并列不占位）
来源：http://apt.cdnleiting.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dvt.bjfxy.top

[Q57] 行号
来源：http://qmx.zhoulong.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xjx.yuanzhike.top

[Q58] 累计求和
来源：http://iee.hnqzz.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vcf.c1oappe.top

[Q59] 分组内累计
来源：http://dsw.c1oappe.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tsf.shanyushiyangkeji.top

[Q60] 取上一行 / 下一行
来源：http://ojg.zhoulong.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ecv.birdmap.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ekx.jinyuanbaomall.cn

[Q61] 移动平均
来源：http://bks.fzhhl.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oda.tian-w.cn

[Q62] 分组占比
来源：http://tqw.yvedp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://abh.bjfxy.top

[Q63] 开启事务
来源：http://wmn.quarkkingdee.top

START TRANSACTION;                -- 或 BEGIN
来源：http://zak.yuxming.cn

[Q64] 提交事务
来源：http://vyi.fanxiaobao.xyz

COMMIT;
来源：http://saj.xylfe.cn

[Q65] 回滚事务
来源：http://qyt.shzxlz.cn

ROLLBACK;
来源：http://lbq.guowangkeji.top

[Q66] 行锁查询
来源：http://eee.chenjidiqi.icu

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lia.tianlin.xyz

[Q67] 设置隔离级别
来源：http://vwj.shangyingyoupin.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hfh.guannengcc.top

[Q68] 保存点
来源：http://vnr.sysykeji.top

SAVEPOINT sp1;
来源：http://xwt.yanxiufei.cn

ROLLBACK TO sp1;
来源：http://ind.bbcook.cn

[Q69] 查看执行计划
来源：http://ncz.cucudq.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qkm.hammf.cn

[Q70] 更新统计信息
来源：http://vmy.hnqzz.top

ANALYZE TABLE users;
来源：http://cdz.hfpthk.cn

[Q71] 查看建表语句
来源：http://gvn.snrcjt.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kab.hysaishi.cn

[Q72] 查看索引
来源：http://yqy.epnwcf.com

SHOW INDEX FROM users;
来源：http://jvo.yonumen.top

[Q73] 查看表状态
来源：http://ylp.sweek.top

SHOW TABLE STATUS LIKE 'users';
来源：http://run.jlsjyb.cn

[Q74] 强制使用索引
来源：http://jyo.haohaochexian.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cap.chenzaomai.com

[Q75] 日期格式化
来源：http://oli.zhongyouzk.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cws.zdqjudy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sbw.xuetiantiany.cn

[Q76] 按天统计
来源：http://ioc.fzhhl.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vgm.uphjek.com

[Q77] 时间加减
来源：http://tat.hywenlv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rch.ydzc1.top

[Q78] 当前时间
来源：http://wnf.nanxinkj.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zcv.cheryme.top

[Q79] 字符串拼接
来源：http://ljv.shangyingyoupin.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bqg.hnxiangtu.top

[Q80] 字符串截取
来源：http://wiu.shanyushiyangtech.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://esc.gotoacloud.top

[Q81] 字符串替换
来源：http://tee.yj20258888.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zpv.yfazqb.com

[Q82] 字符长度与字节长度
来源：http://bak.yanxiufei.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ezt.vehdjk.com

[Q83] 大小写转换
来源：http://lbz.zycfv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zvf.vehdjk.com

[Q84] 去除首尾空格
来源：http://blb.hnqzz.top

SELECT TRIM(name) FROM users;
来源：http://bvh.chenzaomai.com

[Q85] 数值取整
来源：http://vmu.birdmap.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://upt.jinyuanbaomall.cn

[Q86] 读取 JSON 字段
来源：http://bum.feifeiyinyue.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pkz.mhx1999.top

[Q87] JSON 字段做条件
来源：http://uzq.tarul.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kmj.zhongyouzk.top

[Q88] 行转列（条件聚合）
来源：http://qzj.xuanzx.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ekj.gzhubu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sbk.xuetiantiany.cn

[Q89] 判断表是否存在
来源：http://vac.mhx1999.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zxl.fzhhl.top

[Q90] 生成序号列
来源：http://amj.jqgfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://opq.meibo888.top

================================================================================
来源：http://ipr.yuanzhike.top

R. Bash 专题
来源：http://pzw.zhijiandao.cn

================================================================================
来源：http://fet.bbcook.cn

[R01] shebang 与严格模式
来源：http://rsl.cdnleiting.top

#!/usr/bin/env bash
来源：http://jro.tianlin.xyz

set -euo pipefail
来源：http://qaz.shangyingyoupin.top

[R02] 变量赋值与使用
来源：http://zcp.mhx1999.top

name="Tom"; echo "$name"
来源：http://jzp.hfpthk.cn

[R03] 只读变量
来源：http://xkf.snrcjt.cn

readonly PI=3.14
来源：http://svl.316326.xyz

[R04] 位置参数
来源：http://bby.dianchejie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qfc.jiagoushi.top

[R05] 参数默认值
来源：http://nag.chenjidiqi.icu

name="${1:-default}"
来源：http://joq.yongpay.top

[R06] 判断命令是否存在
来源：http://oir.dashuyun.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dmg.jinqigfzy.top

[R07] if 判断文件
来源：http://aiu.kuanghao11.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://exj.kuanghao11.cn

[R08] 数值比较
来源：http://efe.aizwys.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yvf.gzhubu.top

[R09] 字符串比较
来源：http://pds.yj20258888.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kbe.guannengcc.top

[R10] 正则匹配
来源：http://xfi.mhx1999.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cwr.yangfankeji.com

[R11] case 多分支
来源：http://djz.ctjpmb.com

case "$1" in
来源：http://tek.sjlbkw.cn

start) echo "启动" ;;
来源：http://sam.jinqigfzy.top

stop)  echo "停止" ;;
来源：http://tqu.chenlongwang.top

*)     echo "未知命令" ;;
来源：http://ccw.shanyushiyangkeji.top

esac
来源：http://fvd.mhx1999.top

[R12] for 遍历文件
来源：http://szq.gotoacloud.top

for f in *.txt; do echo "$f"; done
来源：http://wri.yonumen.top

[R13] for 计数循环
来源：http://ybj.havefunace.top

for i in {1..10}; do echo "$i"; done
来源：http://vgh.nanxinkj.top

[R14] C 风格 for
来源：http://dxc.zhongyouzk.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cyr.sweek.top

[R15] while 逐行读文件
来源：http://wrz.pengpengdd.cyou

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cxa.fktsv.cn

[R16] until 等待条件
来源：http://ecx.jinyuanbaomall.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://osb.hfpthk.cn

[R17] 数组定义与取值
来源：http://vwz.cashguo.top

arr=(a b c); echo "${arr[0]}"
来源：http://xug.hnqzz.top

[R18] 遍历数组
来源：http://yxp.pengpengdd.cyou

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bfy.yangfankeji.com

[R19] 数组长度
来源：http://trv.xziqi.cn

echo "${#arr[@]}"
来源：http://epc.dianchejie.cn

[R20] 关联数组（字典）
来源：http://lpy.zhaomingkeji.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ooq.ivvv.top

[R21] 字符串长度
来源：http://gfy.bbcook.cn

echo "${#s}"
来源：http://utp.epnwcf.com

[R22] 截取子串
来源：http://yrs.meibo888.top

echo "${s:0:5}"
来源：http://lig.hysaishi.cn

[R23] 字符串替换
来源：http://ebt.bjfxy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ebs.zhiwuduotai.top

[R24] 大小写转换
来源：http://lmb.c1oappe.top

echo "${s^^}"; echo "${s,,}"
来源：http://wed.iojbl.cn

[R25] 去后缀 / 去前缀
来源：http://nsq.0kj1m.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jdv.yongpay.top

[R26] 命令替换
来源：http://pze.wangshuangyany.cn

now=$(date +%F); echo "$now"
来源：http://yzx.gogol.net.cn

[R27] 算术展开
来源：http://jye.sufxvd.cn

echo $((1 + 2 * 3))
来源：http://eyx.zhoulong.xyz

[R28] 浮点运算
来源：http://vgg.bbcook.cn

echo "scale=2; 10/3" | bc
来源：http://hfk.tanke756.top

[R29] 定义函数
来源：http://vvi.jqgufenzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wog.kuanghao11.cn

[R30] 函数返回状态码
来源：http://cco.daxiang520.top

f() { return 0; }; f || echo "失败了"
来源：http://vti.jlsjyb.cn

[R31] 局部变量
来源：http://vdn.mhx1999.top

f() { local x=1; echo "$x"; }
来源：http://dfp.jianghu66.top

[R32] 参数个数校验
来源：http://uhg.fktsv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jyw.sxryk.cn

[R33] 捕获错误并提示行号
来源：http://azh.ivvv.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uxx.hongshengwenyu.top

[R34] 退出时清理
来源：http://kdd.xylfe.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sdt.hongshengwenyu.top

[R35] 后台执行并等待
来源：http://yqz.jyoumei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://oyp.sufxvd.cn

[R36] 并发执行多个任务
来源：http://dxj.zhoulong.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vkj.quarkkingdee.top

[R37] 把输出赋给变量
来源：http://asn.nanxinkj.top

files=$(ls -1)
来源：http://ssg.quarkkingdee.top

[R38] 管道串联
来源：http://tvc.yonumen.top

cat a.txt | grep -i error | wc -l
来源：http://yit.epnwcf.com

[R39] 重定向标准输出与错误
来源：http://mwd.shangyingyoupin.top

cmd > out.log 2>&1
来源：http://ddq.jyoumei.cn

[R40] 追加写日志
来源：http://pgd.jinqigufen.top

echo "log" >> out.log
来源：http://oxo.ydjk.org.cn

[R41] 丢弃输出
来源：http://zzw.ppjwa.cn

cmd >/dev/null 2>&1
来源：http://glo.ydjk.org.cn

[R42] 输入重定向
来源：http://jzt.feifeiyinyue.top

wc -l < a.txt
来源：http://diq.jyoumei.cn

[R43] 按名字查找文件
来源：http://vgq.wangshuangyany.cn

find . -name "*.log" -type f
来源：http://qfe.jqgufenzy.top

[R44] 按修改时间查找
来源：http://bwi.shanyushiyangkeji.top

find . -mtime -7 -type f
来源：http://ewy.zhongyouzk.top

[R45] 批量删除
来源：http://rhu.shanyushiyangkeji.top

find . -name "*.tmp" -delete
来源：http://rpk.zhoulong.xyz

[R46] 递归替换文件内容
来源：http://drw.hnqzz.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://svg.epnwcf.com

[R47] sed 单行替换
来源：http://mlz.jqgfzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://nrk.hywenlv.cn

[R48] awk 取指定列
来源：http://kgz.yueranfly.top

awk '{print $1, $3}' a.txt
来源：http://dga.aizwys.cn

[R49] awk 带条件
来源：http://zml.jlsjyb.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rxg.fengsongda.top

[R50] awk 求和
来源：http://hgj.xziqi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jer.jinqigfzy.top

[R51] 排序去重取前几
来源：http://kqt.ydzc1.top

sort a.txt | uniq -c | sort -rn | head
来源：http://gqv.jyoumei.cn

[R52] 统计行数
来源：http://vdp.haohaochexian.top

wc -l a.txt
来源：http://bqa.316326.xyz

[R53] 查看文件头与实时尾
来源：http://uzr.epnwcf.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://unb.nanxuanxn.top

[R54] 比较两个文件
来源：http://nfr.gaohongyu789.top

diff a.txt b.txt
来源：http://opx.jinghuilouyu.cn

[R55] 压缩与解压
来源：http://zvl.sufxvd.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://agg.bjfxy.top

[R56] 远程拷贝
来源：http://mmv.jqgfzy.top

scp file user@host:/path/
来源：http://nsu.guowangkeji.top

[R57] 远程执行命令
来源：http://cem.hysaishi.cn


<!-- 参考信息 -->