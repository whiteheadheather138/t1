代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://rec.svipenyu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dbn.fanxiaobao.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://knz.hongshengwenyu.top

[Q15] 查询全部
来源：http://uiv.ctjpmb.com

SELECT * FROM users;
来源：http://bev.shzxlz.cn

[Q16] 查询指定列
来源：http://uld.aibaodan.cn

SELECT id, name FROM users;
来源：http://pmq.nanxuanxn.top

[Q17] 条件查询
来源：http://igi.ywan-chungtsiang.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bxo.pengpengdd.cyou

[Q18] 模糊匹配
来源：http://cdp.shuidangran.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kes.cqqwz.cn

[Q19] 范围查询
来源：http://ukk.zhongyouzk.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ksu.52xcode.cn

[Q20] IN 列表
来源：http://mnk.ydzc1.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cxk.ydzc1.top

[Q21] 空值判断
来源：http://jct.bbcook.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bsl.hnqzz.top

[Q22] 排序
来源：http://fdr.epnwcf.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xfb.cdnleiting.top

[Q23] 分页
来源：http://qht.bbcook.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fzr.fengsongda.top

[Q24] 去重
来源：http://ojj.tarul.cn

SELECT DISTINCT city FROM users;
来源：http://prw.smart0.xyz

[Q25] 只取前 N 条
来源：http://xfj.xylfe.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ukm.daria6918.cn

[Q26] 计数
来源：http://bsu.vehdjk.com

SELECT COUNT(*) FROM users;
来源：http://jef.ydjk.org.cn

[Q27] 条件计数
来源：http://fci.jqgufenzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jzd.hongshengwenyu.top

[Q28] 求和与平均
来源：http://gqo.zycfv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bux.nwbrower.top

[Q29] 最大最小值
来源：http://wmg.snrcjt.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ucv.havefunace.top

[Q30] 分组统计
来源：http://bvi.hongshengwenyu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gaz.yj20258888.top

[Q31] 分组后过滤
来源：http://icd.tanke756.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kik.dashuyun.cn

[Q32] 分组拼接字符串
来源：http://bli.yj202588.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eag.yj202588.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ltq.gzhubu.top

[Q33] 多列分组
来源：http://dxv.svipenyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tpl.cashguo.top

[Q34] 每组取第一条
来源：http://coa.jinyuanbaomall.cn

SELECT * FROM (
来源：http://xvp.hammf.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ibn.gogol.net.cn

) t WHERE rn = 1;
来源：http://hhp.dianchejie.cn

[Q35] 内连接
来源：http://xuz.zhixingplan.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gnz.sysykeji.top

[Q36] 左连接
来源：http://uka.xinyue.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ozj.jlsjyb.cn

[Q37] 右连接
来源：http://zkk.daxiang520.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jdz.daria6918.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wbk.jinqigufen.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oda.birdmap.top

[Q39] 自连接（查上下级）
来源：http://nbl.haohaochexian.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://pqi.jiagoushi.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ovl.yongpay.top

[Q40] 交叉连接（笛卡尔积）
来源：http://uge.yueranfly.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yky.9152youxi.cn

[Q41] 多表连接
来源：http://xfg.xylfe.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pgd.nanxuanxn.top

JOIN users u ON u.id = o.user_id
来源：http://usk.bjfxy.top

JOIN products p ON p.id = o.product_id;
来源：http://jag.shangyingyoupin.top

[Q42] 连接条件附加过滤
来源：http://ngj.yanxiufei.cn

SELECT u.name, o.amount FROM users u
来源：http://wid.bbcook.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://oit.zhixingplan.top

[Q43] 标量子查询
来源：http://acm.nwbrower.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://txg.zdqjudy.top

[Q44] IN 子查询
来源：http://qwd.zdqjudy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dur.fzhhl.top

[Q45] EXISTS 判断存在
来源：http://nee.yj202588.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vye.tian-w.cn

[Q46] NOT EXISTS 判断不存在
来源：http://auh.yuxming.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xuj.fengsongda.top

[Q47] 与平均值比较
来源：http://jrk.shanyushiyangtech.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://aej.meibo888.top

[Q48] CTE 公用表表达式
来源：http://ifp.snrcjt.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bnv.tian-w.cn

SELECT * FROM t WHERE c > 5;
来源：http://hqz.sweek.top

[Q49] 更新单行
来源：http://cdc.yvedp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dat.cucudq.cn

[Q50] 批量更新
来源：http://wdg.fengsongda.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cqt.hesvh.cn

[Q51] 用子查询更新
来源：http://obb.tanke756.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vqc.gzhubu.top

[Q52] 删除指定行
来源：http://ign.ehwqpu.com

DELETE FROM users WHERE id = 10;
来源：http://yhn.jlsjyb.cn

[Q53] 按条件删除
来源：http://axe.tarul.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kac.yanxiufei.cn

[Q54] 清空表
来源：http://tig.snrcjt.cn

TRUNCATE TABLE logs;
来源：http://zrl.fehbvm.com

[Q55] 排名（并列占位）
来源：http://xdu.aizwys.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zfx.yangfankeji.com

[Q56] 密集排名（并列不占位）
来源：http://dkk.zycfv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dsy.daria6918.cn

[Q57] 行号
来源：http://ouu.shanyushiyangkeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://iwe.zhijiandao.cn

[Q58] 累计求和
来源：http://ffj.0kj1m.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kmv.shzxlz.cn

[Q59] 分组内累计
来源：http://vrp.yongpay.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wgl.9152youxi.cn

[Q60] 取上一行 / 下一行
来源：http://vuu.yongpay.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uvz.shuidangran.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ojc.yangfankeji.com

[Q61] 移动平均
来源：http://oiv.yangfankeji.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sts.chenzaomai.com

[Q62] 分组占比
来源：http://ese.guannengcc.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uly.sxryk.cn

[Q63] 开启事务
来源：http://rsq.yanxiufei.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wue.xinyue.icu

[Q64] 提交事务
来源：http://ptj.xinyue.icu

COMMIT;
来源：http://umx.tianlin.xyz

[Q65] 回滚事务
来源：http://okp.ehwqpu.com

ROLLBACK;
来源：http://hng.ybcxt.top

[Q66] 行锁查询
来源：http://sdn.gogol.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wtv.tarul.cn

[Q67] 设置隔离级别
来源：http://qlk.mhx1999.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jlw.guowangkeji.top

[Q68] 保存点
来源：http://pag.vqdsnc.cn

SAVEPOINT sp1;
来源：http://dmh.wangdashe.top

ROLLBACK TO sp1;
来源：http://cvr.quarkkingdee.top

[Q69] 查看执行计划
来源：http://pzr.shangyingyoupin.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rvb.shanyushiyangtech.top

[Q70] 更新统计信息
来源：http://ejb.daxiang520.top

ANALYZE TABLE users;
来源：http://glf.nwbrower.top

[Q71] 查看建表语句
来源：http://mjc.chenzaomai.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://esi.shzxlz.cn

[Q72] 查看索引
来源：http://nzi.0kj1m.cn

SHOW INDEX FROM users;
来源：http://frj.0kj1m.cn

[Q73] 查看表状态
来源：http://onw.xingfuxueyuan.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://ltr.feifeiyinyue.top

[Q74] 强制使用索引
来源：http://wvz.fehbvm.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qsj.zhongyouzk.top

[Q75] 日期格式化
来源：http://mro.sysykeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kgb.tianlin.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vrv.jlsjyb.cn

[Q76] 按天统计
来源：http://hhi.guannengcc.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rok.fzhhl.top

[Q77] 时间加减
来源：http://nmn.chenjidiqi.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qlb.chenjidiqi.icu

[Q78] 当前时间
来源：http://mlm.jinyuanbaomall.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kqh.vehdjk.com

[Q79] 字符串拼接
来源：http://mqd.daxiang520.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sqr.hfpthk.cn

[Q80] 字符串截取
来源：http://wsg.shzxlz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gli.gotoacloud.top

[Q81] 字符串替换
来源：http://gjm.vqdsnc.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lbo.yj20258.top

[Q82] 字符长度与字节长度
来源：http://ivg.zhiwuduotai.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jzf.zhongyouzk.top

[Q83] 大小写转换
来源：http://tvm.epnwcf.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zek.fanxiaobao.xyz

[Q84] 去除首尾空格
来源：http://typ.yuxming.cn

SELECT TRIM(name) FROM users;
来源：http://vzk.fktsv.cn

[Q85] 数值取整
来源：http://xmj.yj202588.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tdu.9152youxi.cn

[Q86] 读取 JSON 字段
来源：http://ytz.daxiang520.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qbf.birdmap.top

[Q87] JSON 字段做条件
来源：http://etf.zhijiandao.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rdv.nanxuanxn.top

[Q88] 行转列（条件聚合）
来源：http://wcl.cqqwz.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ubh.hfpthk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fpt.uphjek.com

[Q89] 判断表是否存在
来源：http://npo.hcnkem.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pml.chenlongwang.top

[Q90] 生成序号列
来源：http://kxz.haohaochexian.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://evt.gotoacloud.top

================================================================================
来源：http://bbg.jinqigufen.top

R. Bash 专题
来源：http://ntq.hcnkem.com

================================================================================
来源：http://cca.zycfv.cn

[R01] shebang 与严格模式
来源：http://dtj.shangyingyoupin.top

#!/usr/bin/env bash
来源：http://glo.c1oappe.top

set -euo pipefail
来源：http://bpg.feifeiyinyue.top

[R02] 变量赋值与使用
来源：http://nmy.ehwqpu.com

name="Tom"; echo "$name"
来源：http://dik.chenjidiqi.icu

[R03] 只读变量
来源：http://xjn.shanyushiyangtech.top

readonly PI=3.14
来源：http://lxt.haohaochexian.top

[R04] 位置参数
来源：http://sgi.wangshuangyany.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ert.kuanghao11.cn

[R05] 参数默认值
来源：http://wyo.dianchejie.cn

name="${1:-default}"
来源：http://wgn.svipenyu.cn

[R06] 判断命令是否存在
来源：http://wfy.shanyushiyangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://oat.jianghu66.top

[R07] if 判断文件
来源：http://ywp.pengpengdd.cyou

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ihk.tianlin.xyz

[R08] 数值比较
来源：http://kbc.chenjidiqi.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://vvr.nanxinkj.top

[R09] 字符串比较
来源：http://zjr.0kj1m.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kww.yuanzhike.top

[R10] 正则匹配
来源：http://zth.xziqi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://buq.bbcook.cn

[R11] case 多分支
来源：http://lli.gogol.net.cn

case "$1" in
来源：http://woo.tian-w.cn

start) echo "启动" ;;
来源：http://tii.ybcxt.top

stop)  echo "停止" ;;
来源：http://joh.zycfv.cn

*)     echo "未知命令" ;;
来源：http://wmc.hnxiangtu.top

esac
来源：http://ljj.tianlin.xyz

[R12] for 遍历文件
来源：http://kgi.zhoulong.xyz

for f in *.txt; do echo "$f"; done
来源：http://yme.uphjek.com

[R13] for 计数循环
来源：http://irr.quarkkingdee.top

for i in {1..10}; do echo "$i"; done
来源：http://lzp.yj202588.top

[R14] C 风格 for
来源：http://svd.pycfn.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zhw.yj20258888.top

[R15] while 逐行读文件
来源：http://rry.hesvh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://npz.jinyuanbaomall.cn

[R16] until 等待条件
来源：http://qnq.gzhubu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uqe.hfpthk.cn

[R17] 数组定义与取值
来源：http://thh.havefunace.top

arr=(a b c); echo "${arr[0]}"
来源：http://apg.hcnkem.com

[R18] 遍历数组
来源：http://cjz.hongshengwenyu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zpj.9152youxi.cn

[R19] 数组长度
来源：http://qwa.316326.xyz

echo "${#arr[@]}"
来源：http://zni.ywan-chungtsiang.top

[R20] 关联数组（字典）
来源：http://ecl.vehdjk.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xel.gotoacloud.top

[R21] 字符串长度
来源：http://uxw.gotoacloud.top

echo "${#s}"
来源：http://qxv.epnwcf.com

[R22] 截取子串
来源：http://vut.shuidangran.top

echo "${s:0:5}"
来源：http://wtm.yfazqb.com

[R23] 字符串替换
来源：http://xxf.hywenlv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ppv.xziqi.cn

[R24] 大小写转换
来源：http://mdc.cashguo.top

echo "${s^^}"; echo "${s,,}"
来源：http://dlo.sufxvd.cn

[R25] 去后缀 / 去前缀
来源：http://pzv.hysaishi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bgb.kuanghao11.cn

[R26] 命令替换
来源：http://wfl.zhongyouzk.top

now=$(date +%F); echo "$now"
来源：http://svk.ydjk.org.cn

[R27] 算术展开
来源：http://ssu.ppjwa.cn

echo $((1 + 2 * 3))
来源：http://hve.hnqzz.top

[R28] 浮点运算
来源：http://zyr.daria6918.cn

echo "scale=2; 10/3" | bc
来源：http://lke.nwbrower.top

[R29] 定义函数
来源：http://unv.zhaomingkeji.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oec.chenjidiqi.icu

[R30] 函数返回状态码
来源：http://hfb.zdqjudy.top

f() { return 0; }; f || echo "失败了"
来源：http://gxy.cheryme.top

[R31] 局部变量
来源：http://rjt.gogol.net.cn

f() { local x=1; echo "$x"; }
来源：http://hmh.dianchejie.cn

[R32] 参数个数校验
来源：http://pbq.gogol.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bld.sweek.top

[R33] 捕获错误并提示行号
来源：http://sgv.shanyushiyangkeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rkq.svipenyu.cn

[R34] 退出时清理
来源：http://jdp.tanke756.top

trap 'rm -f "$tmp"' EXIT
来源：http://noy.hammf.cn

[R35] 后台执行并等待
来源：http://zao.316326.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://xuo.yuxming.cn

[R36] 并发执行多个任务
来源：http://ihb.vehdjk.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pec.dashuyun.cn

[R37] 把输出赋给变量
来源：http://gnu.shuidangran.top

files=$(ls -1)
来源：http://cjr.c1oappe.top

[R38] 管道串联
来源：http://wmn.zhoulong.xyz

cat a.txt | grep -i error | wc -l
来源：http://axc.zhongyouzk.top

[R39] 重定向标准输出与错误
来源：http://ujx.xziqi.cn

cmd > out.log 2>&1
来源：http://krt.hysaishi.cn

[R40] 追加写日志
来源：http://res.yonumen.top

echo "log" >> out.log
来源：http://blb.hongshengwenyu.top

[R41] 丢弃输出
来源：http://evj.andypj.xyz

cmd >/dev/null 2>&1
来源：http://bvk.hammf.cn

[R42] 输入重定向
来源：http://kso.ydzc1.top

wc -l < a.txt
来源：http://nve.0kj1m.cn

[R43] 按名字查找文件
来源：http://tbd.tarul.cn

find . -name "*.log" -type f
来源：http://trp.epnwcf.com

[R44] 按修改时间查找
来源：http://sst.jyoumei.cn

find . -mtime -7 -type f
来源：http://tkj.yj20258.top

[R45] 批量删除
来源：http://tqc.nwbrower.top

find . -name "*.tmp" -delete
来源：http://sad.yangfankeji.com

[R46] 递归替换文件内容
来源：http://uzi.cdnleiting.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ydk.fktsv.cn

[R47] sed 单行替换
来源：http://zge.yonumen.top

sed -i 's/foo/bar/g' a.txt
来源：http://pbc.zdqjudy.top

[R48] awk 取指定列
来源：http://fpw.guannengcc.top

awk '{print $1, $3}' a.txt
来源：http://muw.andypj.xyz

[R49] awk 带条件
来源：http://jhw.jlsjyb.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rit.yanxiufei.cn

[R50] awk 求和
来源：http://pyg.hfpthk.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kwh.fzhhl.top

[R51] 排序去重取前几
来源：http://oua.yj20258.top

sort a.txt | uniq -c | sort -rn | head
来源：http://toh.bjfxy.top

[R52] 统计行数
来源：http://hqg.chenzaomai.com

wc -l a.txt
来源：http://zsr.ctjpmb.com

[R53] 查看文件头与实时尾
来源：http://ptx.gogol.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lrm.jqgfzy.top

[R54] 比较两个文件
来源：http://ksl.cashguo.top

diff a.txt b.txt
来源：http://zbt.cheryme.top

[R55] 压缩与解压
来源：http://vdv.cdnleiting.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ylj.xziqi.cn

[R56] 远程拷贝
来源：http://awe.sjlbkw.cn

scp file user@host:/path/
来源：http://pqe.ywan-chungtsiang.top

[R57] 远程执行命令
来源：http://oyt.gaohongyu789.top

ssh user@host 'uptime'
来源：http://ocd.pycfn.com

[R58] 下载文件
来源：http://zjo.epnwcf.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ewn.yuxming.cn

[R59] 发 POST JSON
来源：http://muj.shangyingyoupin.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cvy.sysykeji.top

[R60] 只看 HTTP 状态码
来源：http://eek.yueranfly.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vid.quarkkingdee.top

[R61] 磁盘占用
来源：http://glp.cheryme.top

df -h;  du -sh *
来源：http://olh.jinqigfzy.top

[R62] 找最占空间的文件
来源：http://ysr.jqgufenzy.top

du -ah . | sort -rh | head -10
来源：http://dqk.uphjek.com

[R63] 内存与进程
来源：http://kxc.fehbvm.com


<!-- 参考信息 -->