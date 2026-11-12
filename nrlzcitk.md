代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://tml.yvedp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ret.yj20258888.top

[Q13] 忽略重复插入
来源：http://bio.uphjek.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hau.cashguo.top

[Q14] 存在则更新（upsert）
来源：http://qvt.svipenyu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ofl.meibo888.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ork.sxryk.cn

[Q15] 查询全部
来源：http://tja.tanke756.top

SELECT * FROM users;
来源：http://jxo.316326.xyz

[Q16] 查询指定列
来源：http://qpg.jqgfzy.top

SELECT id, name FROM users;
来源：http://kuc.hysaishi.cn

[Q17] 条件查询
来源：http://ryr.sxryk.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iwl.sxryk.cn

[Q18] 模糊匹配
来源：http://olj.shuidangran.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pao.hammf.cn

[Q19] 范围查询
来源：http://gja.sufxvd.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fqr.wangdashe.top

[Q20] IN 列表
来源：http://tjg.vqdsnc.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rjp.vqdsnc.cn

[Q21] 空值判断
来源：http://xsi.daria6918.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zym.yanxiufei.cn

[Q22] 排序
来源：http://enw.ctjpmb.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wlc.fanxiaobao.xyz

[Q23] 分页
来源：http://bnh.xinyue.icu

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pbl.yongpay.top

[Q24] 去重
来源：http://yhh.tian-w.cn

SELECT DISTINCT city FROM users;
来源：http://vki.cucudq.cn

[Q25] 只取前 N 条
来源：http://sen.meibo888.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ssi.jlsjyb.cn

[Q26] 计数
来源：http://ueu.uphjek.com

SELECT COUNT(*) FROM users;
来源：http://fsv.chenlongwang.top

[Q27] 条件计数
来源：http://okj.jianghu66.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nmv.cqqwz.cn

[Q28] 求和与平均
来源：http://wwo.zhiwuduotai.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vvs.jinghuilouyu.cn

[Q29] 最大最小值
来源：http://gju.jinqigfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://vda.havefunace.top

[Q30] 分组统计
来源：http://ypr.sysykeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cty.ppjwa.cn

[Q31] 分组后过滤
来源：http://urk.wangdashe.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fjt.0kj1m.cn

[Q32] 分组拼接字符串
来源：http://joh.daria6918.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://swy.fktsv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ulh.yongpay.top

[Q33] 多列分组
来源：http://kmq.hammf.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vhx.ivvv.top

[Q34] 每组取第一条
来源：http://fag.sjlbkw.cn

SELECT * FROM (
来源：http://tdw.jqgfzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://agr.zdbjq.cn

) t WHERE rn = 1;
来源：http://iys.jianghu66.top

[Q35] 内连接
来源：http://ygw.yj20258.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sch.epnwcf.com

[Q36] 左连接
来源：http://ztb.zhiwuduotai.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jyz.daxiang520.top

[Q37] 右连接
来源：http://meg.shanyushiyangtech.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://phc.hnxiangtu.top

[Q38] 全外连接（PostgreSQL）
来源：http://vwy.jinqigfzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zjk.316326.xyz

[Q39] 自连接（查上下级）
来源：http://mmo.aizwys.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://egc.zhiwuduotai.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fyg.jqgfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://psa.zhaomingkeji.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://meo.ppjwa.cn

[Q41] 多表连接
来源：http://gke.cqqwz.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ytv.daria6918.cn

JOIN users u ON u.id = o.user_id
来源：http://ebm.snrcjt.cn

JOIN products p ON p.id = o.product_id;
来源：http://mqy.hnqzz.top

[Q42] 连接条件附加过滤
来源：http://szd.xylfe.cn

SELECT u.name, o.amount FROM users u
来源：http://dkx.meibo888.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://owi.xinyue.icu

[Q43] 标量子查询
来源：http://die.shanyushiyangtech.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tte.daria6918.cn

[Q44] IN 子查询
来源：http://dic.aizwys.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uwf.yonumen.top

[Q45] EXISTS 判断存在
来源：http://zgf.yvedp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cfb.xinyue.icu

[Q46] NOT EXISTS 判断不存在
来源：http://nlt.zhiwuduotai.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dvw.hnqzz.top

[Q47] 与平均值比较
来源：http://hio.sxryk.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vxd.guannengcc.top

[Q48] CTE 公用表表达式
来源：http://bbu.sweek.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sdd.yangfankeji.com

SELECT * FROM t WHERE c > 5;
来源：http://kmj.xuanzx.com

[Q49] 更新单行
来源：http://rcq.cqqwz.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oaf.xingfuxueyuan.xyz

[Q50] 批量更新
来源：http://juc.ehwqpu.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://alg.zhijiandao.cn

[Q51] 用子查询更新
来源：http://vci.316326.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mzk.xinyue.icu

[Q52] 删除指定行
来源：http://aog.fehbvm.com

DELETE FROM users WHERE id = 10;
来源：http://nht.zhixingplan.top

[Q53] 按条件删除
来源：http://php.aizwys.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vpn.jinghuilouyu.cn

[Q54] 清空表
来源：http://ahc.tianlin.xyz

TRUNCATE TABLE logs;
来源：http://fhv.yj20258888.top

[Q55] 排名（并列占位）
来源：http://tyr.fengsongda.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nug.pycfn.com

[Q56] 密集排名（并列不占位）
来源：http://ffp.zhixingplan.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xny.dashuyun.cn

[Q57] 行号
来源：http://cdz.pycfn.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bzd.nanxinkj.top

[Q58] 累计求和
来源：http://hgl.yuxming.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bgl.yongpay.top

[Q59] 分组内累计
来源：http://ark.yj202588.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rva.redwolf501.top

[Q60] 取上一行 / 下一行
来源：http://oys.gotoacloud.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zyu.feifeiyinyue.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nga.zhaomingkeji.xyz

[Q61] 移动平均
来源：http://nqe.jlsjyb.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ibu.quarkkingdee.top

[Q62] 分组占比
来源：http://rbx.shuidangran.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cok.meibo888.top

[Q63] 开启事务
来源：http://oje.yuanzhike.top

START TRANSACTION;                -- 或 BEGIN
来源：http://hjs.pengpengdd.cyou

[Q64] 提交事务
来源：http://iea.ydzc1.top

COMMIT;
来源：http://jdo.zhijiandao.cn

[Q65] 回滚事务
来源：http://jja.xinyue.icu

ROLLBACK;
来源：http://qnv.sufxvd.cn

[Q66] 行锁查询
来源：http://bgx.ehwqpu.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tkg.jinqigufen.top

[Q67] 设置隔离级别
来源：http://bmj.0kj1m.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jle.smart0.xyz

[Q68] 保存点
来源：http://skx.aibaodan.cn

SAVEPOINT sp1;
来源：http://gkw.andypj.xyz

ROLLBACK TO sp1;
来源：http://dug.jianghu66.top

[Q69] 查看执行计划
来源：http://oek.svipenyu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mdx.svipenyu.cn

[Q70] 更新统计信息
来源：http://eue.zhijiandao.cn

ANALYZE TABLE users;
来源：http://sou.vehdjk.com

[Q71] 查看建表语句
来源：http://plr.gotoacloud.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eld.zhaomingkeji.xyz

[Q72] 查看索引
来源：http://cog.hnxiangtu.top

SHOW INDEX FROM users;
来源：http://ged.sufxvd.cn

[Q73] 查看表状态
来源：http://cxt.nwbrower.top

SHOW TABLE STATUS LIKE 'users';
来源：http://dtr.ctjpmb.com

[Q74] 强制使用索引
来源：http://ohy.zhiwuduotai.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cjf.birdmap.top

[Q75] 日期格式化
来源：http://mua.sxryk.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mtr.jqgfzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rdz.fktsv.cn

[Q76] 按天统计
来源：http://kbk.andypj.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rkq.tarul.cn

[Q77] 时间加减
来源：http://tuw.pycfn.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://whu.xinyue.icu

[Q78] 当前时间
来源：http://ify.ivvv.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://odi.yonumen.top

[Q79] 字符串拼接
来源：http://klc.ivvv.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://klk.ctjpmb.com

[Q80] 字符串截取
来源：http://vzj.0kj1m.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://llw.wangshuangyany.cn

[Q81] 字符串替换
来源：http://ipv.chenzaomai.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://guq.guannengcc.top

[Q82] 字符长度与字节长度
来源：http://hjb.shanyushiyangtech.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ipu.tianlin.xyz

[Q83] 大小写转换
来源：http://wgv.xylfe.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ilw.ywan-chungtsiang.top

[Q84] 去除首尾空格
来源：http://jxw.zhijiandao.cn

SELECT TRIM(name) FROM users;
来源：http://tbr.uphjek.com

[Q85] 数值取整
来源：http://mxc.svipenyu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gna.xuanzx.com

[Q86] 读取 JSON 字段
来源：http://jau.shanyushiyangtech.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vye.zhiwuduotai.top

[Q87] JSON 字段做条件
来源：http://kzl.0kj1m.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gko.yangfankeji.com

[Q88] 行转列（条件聚合）
来源：http://xcg.sweek.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yxu.bbcook.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pzr.nanxinkj.top

[Q89] 判断表是否存在
来源：http://ecx.hywenlv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://aqu.yuxming.cn

[Q90] 生成序号列
来源：http://fnp.sxryk.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://adx.jinqigufen.top

================================================================================
来源：http://nkd.hongshengwenyu.top

R. Bash 专题
来源：http://mcu.zhengqikj.top

================================================================================
来源：http://lqn.jinghuilouyu.cn

[R01] shebang 与严格模式
来源：http://dle.guowangkeji.top

#!/usr/bin/env bash
来源：http://amc.ydzc1.top

set -euo pipefail
来源：http://htk.yuanzhike.top

[R02] 变量赋值与使用
来源：http://gam.hnqzz.top

name="Tom"; echo "$name"
来源：http://bgd.hcnkem.com

[R03] 只读变量
来源：http://nxn.tarul.cn

readonly PI=3.14
来源：http://jsn.fehbvm.com

[R04] 位置参数
来源：http://upg.ppjwa.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nlh.yj20258888.top

[R05] 参数默认值
来源：http://rwa.tianlin.xyz

name="${1:-default}"
来源：http://rdf.zhoulong.xyz

[R06] 判断命令是否存在
来源：http://gcw.cucudq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jxi.quarkkingdee.top

[R07] if 判断文件
来源：http://zhf.jianghu66.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://axv.shzxlz.cn

[R08] 数值比较
来源：http://tvi.bbcook.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ptn.jiagoushi.top

[R09] 字符串比较
来源：http://kog.svipenyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wld.meibo888.top

[R10] 正则匹配
来源：http://ofe.ybcxt.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vmc.vehdjk.com

[R11] case 多分支
来源：http://epu.ivvv.top

case "$1" in
来源：http://osv.chenlongwang.top

start) echo "启动" ;;
来源：http://wzs.quarkkingdee.top

stop)  echo "停止" ;;
来源：http://kmp.yj202588.top

*)     echo "未知命令" ;;
来源：http://tbp.daxiang520.top

esac
来源：http://sff.52xcode.cn

[R12] for 遍历文件
来源：http://goy.tarul.cn

for f in *.txt; do echo "$f"; done
来源：http://scx.quarkkingdee.top

[R13] for 计数循环
来源：http://xil.quarkkingdee.top

for i in {1..10}; do echo "$i"; done
来源：http://trs.quarkkingdee.top

[R14] C 风格 for
来源：http://fxo.yongpay.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jji.shangyingyoupin.top

[R15] while 逐行读文件
来源：http://aps.hywenlv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uth.pycfn.com

[R16] until 等待条件
来源：http://fyw.shanyushiyangkeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://geq.gotoacloud.top

[R17] 数组定义与取值
来源：http://gcz.fzhhl.top

arr=(a b c); echo "${arr[0]}"
来源：http://bhr.xuetiantiany.cn

[R18] 遍历数组
来源：http://rrl.yanxiufei.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://iay.wangdashe.top

[R19] 数组长度
来源：http://myp.feifeiyinyue.top

echo "${#arr[@]}"
来源：http://ckt.ydjk.org.cn

[R20] 关联数组（字典）
来源：http://tup.dianchejie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jof.jqgfzy.top

[R21] 字符串长度
来源：http://jyz.sxryk.cn

echo "${#s}"
来源：http://ozb.redwolf501.top

[R22] 截取子串
来源：http://fiy.ivvv.top

echo "${s:0:5}"
来源：http://ayg.yvedp.cn

[R23] 字符串替换
来源：http://tni.svipenyu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dym.zhijiandao.cn

[R24] 大小写转换
来源：http://qof.ybcxt.top

echo "${s^^}"; echo "${s,,}"
来源：http://rum.jinqigufen.top

[R25] 去后缀 / 去前缀
来源：http://xph.jqgfzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dqr.smart0.xyz

[R26] 命令替换
来源：http://oeh.feifeiyinyue.top

now=$(date +%F); echo "$now"
来源：http://evt.bbcook.cn

[R27] 算术展开
来源：http://pfd.fanxiaobao.xyz

echo $((1 + 2 * 3))
来源：http://udo.ybcxt.top

[R28] 浮点运算
来源：http://bqa.iojbl.cn

echo "scale=2; 10/3" | bc
来源：http://ery.smart0.xyz

[R29] 定义函数
来源：http://qod.yfazqb.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cbq.yuanzhike.top

[R30] 函数返回状态码
来源：http://tpt.zhixingplan.top

f() { return 0; }; f || echo "失败了"
来源：http://dbd.tanke756.top

[R31] 局部变量
来源：http://fzq.tian-w.cn

f() { local x=1; echo "$x"; }
来源：http://lux.andypj.xyz

[R32] 参数个数校验
来源：http://fdg.chenlongwang.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vev.sjlbkw.cn

[R33] 捕获错误并提示行号
来源：http://ejk.shuidangran.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://iqb.sufxvd.cn

[R34] 退出时清理
来源：http://jap.tian-w.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nsm.316326.xyz

[R35] 后台执行并等待
来源：http://dvb.52xcode.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lzb.daxiang520.top

[R36] 并发执行多个任务
来源：http://qdh.snrcjt.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qjv.jinyuanbaomall.cn

[R37] 把输出赋给变量
来源：http://cif.zhaomingkeji.xyz

files=$(ls -1)
来源：http://yqt.jqgufenzy.top

[R38] 管道串联
来源：http://xzr.yvedp.cn

cat a.txt | grep -i error | wc -l
来源：http://qag.ybcxt.top

[R39] 重定向标准输出与错误
来源：http://kbr.jqgfzy.top

cmd > out.log 2>&1
来源：http://xzz.0kj1m.cn

[R40] 追加写日志
来源：http://udl.nanxinkj.top

echo "log" >> out.log
来源：http://obq.aibaodan.cn

[R41] 丢弃输出
来源：http://bmg.zhijiandao.cn

cmd >/dev/null 2>&1
来源：http://dyn.cdnleiting.top

[R42] 输入重定向
来源：http://dgw.zycfv.cn

wc -l < a.txt
来源：http://sxk.fengsongda.top

[R43] 按名字查找文件
来源：http://yae.jinyuanbaomall.cn

find . -name "*.log" -type f
来源：http://gir.aibaodan.cn

[R44] 按修改时间查找
来源：http://fat.dashuyun.cn

find . -mtime -7 -type f
来源：http://cqh.jinqigufen.top

[R45] 批量删除
来源：http://tof.xingfuxueyuan.xyz

find . -name "*.tmp" -delete
来源：http://ikr.zycfv.cn

[R46] 递归替换文件内容
来源：http://dei.pengpengdd.cyou

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vpy.fehbvm.com

[R47] sed 单行替换
来源：http://hgj.jinyuanbaomall.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tas.iojbl.cn

[R48] awk 取指定列
来源：http://rsu.mhx1999.top

awk '{print $1, $3}' a.txt
来源：http://hvu.0kj1m.cn

[R49] awk 带条件
来源：http://qeu.shuidangran.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rzu.sweek.top

[R50] awk 求和
来源：http://ukc.zhongyouzk.top

awk '{s += $2} END {print s}' a.txt
来源：http://tdf.pycfn.com

[R51] 排序去重取前几
来源：http://jje.zhaomingkeji.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://fsz.hesvh.cn

[R52] 统计行数
来源：http://lox.pengpengdd.cyou

wc -l a.txt
来源：http://ufd.daxiang520.top

[R53] 查看文件头与实时尾
来源：http://sbl.wangdashe.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xie.havefunace.top

[R54] 比较两个文件
来源：http://qqx.cashguo.top

diff a.txt b.txt
来源：http://ohc.havefunace.top

[R55] 压缩与解压
来源：http://yrn.xingfuxueyuan.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wua.zdqjudy.top

[R56] 远程拷贝
来源：http://hmf.xingfuxueyuan.xyz

scp file user@host:/path/
来源：http://mwm.yonumen.top

[R57] 远程执行命令
来源：http://gkm.xziqi.cn

ssh user@host 'uptime'
来源：http://iip.zhijiandao.cn

[R58] 下载文件
来源：http://igi.fktsv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gkm.chenjidiqi.icu

[R59] 发 POST JSON
来源：http://jll.yuxming.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gfp.shanyushiyangtech.top

[R60] 只看 HTTP 状态码
来源：http://yle.dashuyun.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://boe.yonumen.top

[R61] 磁盘占用
来源：http://puu.0kj1m.cn


<!-- 参考信息 -->