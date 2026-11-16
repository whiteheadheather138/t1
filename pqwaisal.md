代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://ukr.snrcjt.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mim.zdqjudy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://syk.jianghu66.top

[Q15] 查询全部
来源：http://gcj.bjfxy.top

SELECT * FROM users;
来源：http://xot.snrcjt.cn

[Q16] 查询指定列
来源：http://klc.kuanghao11.cn

SELECT id, name FROM users;
来源：http://qkz.tanke756.top

[Q17] 条件查询
来源：http://ouw.zhongyouzk.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://idl.gotoacloud.top

[Q18] 模糊匹配
来源：http://inv.nanxuanxn.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tyo.hysaishi.cn

[Q19] 范围查询
来源：http://txb.yonumen.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nxy.fktsv.cn

[Q20] IN 列表
来源：http://qsz.zdbjq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://apj.gotoacloud.top

[Q21] 空值判断
来源：http://yim.9152youxi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sbi.vehdjk.com

[Q22] 排序
来源：http://ixo.haohaochexian.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kcy.quarkkingdee.top

[Q23] 分页
来源：http://prs.jianghu66.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hxv.dianchejie.cn

[Q24] 去重
来源：http://zof.redwolf501.top

SELECT DISTINCT city FROM users;
来源：http://lhi.ydjk.org.cn

[Q25] 只取前 N 条
来源：http://cxs.guannengcc.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sjl.tarul.cn

[Q26] 计数
来源：http://kyw.yfazqb.com

SELECT COUNT(*) FROM users;
来源：http://xux.redwolf501.top

[Q27] 条件计数
来源：http://dwz.yangfankeji.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iik.ydzc1.top

[Q28] 求和与平均
来源：http://wje.shanyushiyangtech.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pcb.snrcjt.cn

[Q29] 最大最小值
来源：http://bng.zhongyouzk.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://uxb.ehwqpu.com

[Q30] 分组统计
来源：http://yqz.xinyue.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jkx.hfpthk.cn

[Q31] 分组后过滤
来源：http://raj.kuanghao11.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gbe.cucudq.cn

[Q32] 分组拼接字符串
来源：http://xvt.gogol.net.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://osu.dianchejie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yai.zycfv.cn

[Q33] 多列分组
来源：http://plw.tianlin.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://suw.hnqzz.top

[Q34] 每组取第一条
来源：http://sgl.zhongyouzk.top

SELECT * FROM (
来源：http://dgr.shangyingyoupin.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zqk.xingfuxueyuan.xyz

) t WHERE rn = 1;
来源：http://xon.haohaochexian.top

[Q35] 内连接
来源：http://cqq.guannengcc.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://atl.yueranfly.top

[Q36] 左连接
来源：http://uec.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qec.uphjek.com

[Q37] 右连接
来源：http://nes.zhijiandao.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yot.ehwqpu.com

[Q38] 全外连接（PostgreSQL）
来源：http://cbd.316326.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dik.sufxvd.cn

[Q39] 自连接（查上下级）
来源：http://gmb.chenzaomai.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://ibm.jqgufenzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://khl.wangshuangyany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://aen.tarul.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rwy.yueranfly.top

[Q41] 多表连接
来源：http://kzl.0kj1m.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://kzp.yj202588.top

JOIN users u ON u.id = o.user_id
来源：http://xuu.sysykeji.top

JOIN products p ON p.id = o.product_id;
来源：http://wea.iojbl.cn

[Q42] 连接条件附加过滤
来源：http://wnz.sxryk.cn

SELECT u.name, o.amount FROM users u
来源：http://nuk.hongshengwenyu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://eqy.ydzc1.top

[Q43] 标量子查询
来源：http://yjg.sweek.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zkb.zdqjudy.top

[Q44] IN 子查询
来源：http://rdq.feifeiyinyue.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cae.yj202588.top

[Q45] EXISTS 判断存在
来源：http://ndb.havefunace.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bjq.hysaishi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vqq.shanyushiyangtech.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cyp.hesvh.cn

[Q47] 与平均值比较
来源：http://dbk.sxryk.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ajg.zhaomingkeji.xyz

[Q48] CTE 公用表表达式
来源：http://xae.bjfxy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xyf.sysykeji.top

SELECT * FROM t WHERE c > 5;
来源：http://ebc.zhijiandao.cn

[Q49] 更新单行
来源：http://juw.zdqjudy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wie.havefunace.top

[Q50] 批量更新
来源：http://wdh.jinqigufen.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ucr.redwolf501.top

[Q51] 用子查询更新
来源：http://rwa.xingfuxueyuan.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nro.shanyushiyangkeji.top

[Q52] 删除指定行
来源：http://dkk.ppjwa.cn

DELETE FROM users WHERE id = 10;
来源：http://faw.gogol.net.cn

[Q53] 按条件删除
来源：http://upy.yonumen.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kwz.daxiang520.top

[Q54] 清空表
来源：http://wrv.zycfv.cn

TRUNCATE TABLE logs;
来源：http://fsi.chenjidiqi.icu

[Q55] 排名（并列占位）
来源：http://iyu.zhengqikj.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pmw.fzhhl.top

[Q56] 密集排名（并列不占位）
来源：http://bew.c1oappe.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rov.yueranfly.top

[Q57] 行号
来源：http://ndw.mhx1999.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ukb.shangyingyoupin.top

[Q58] 累计求和
来源：http://hko.ybcxt.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hdi.pengpengdd.cyou

[Q59] 分组内累计
来源：http://qkz.hammf.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bwm.dashuyun.cn

[Q60] 取上一行 / 下一行
来源：http://wfn.hongshengwenyu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jge.cqqwz.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zlx.zhiwuduotai.top

[Q61] 移动平均
来源：http://uag.andypj.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kwk.yuxming.cn

[Q62] 分组占比
来源：http://xwr.guannengcc.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mqp.xingfuxueyuan.xyz

[Q63] 开启事务
来源：http://wxc.gzhubu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ujr.chenlongwang.top

[Q64] 提交事务
来源：http://hzp.havefunace.top

COMMIT;
来源：http://umf.zhijiandao.cn

[Q65] 回滚事务
来源：http://hzn.ivvv.top

ROLLBACK;
来源：http://gfl.tanke756.top

[Q66] 行锁查询
来源：http://xok.haohaochexian.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://saj.sufxvd.cn

[Q67] 设置隔离级别
来源：http://qxe.hesvh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hsd.jqgfzy.top

[Q68] 保存点
来源：http://icj.wangshuangyany.cn

SAVEPOINT sp1;
来源：http://daa.uphjek.com

ROLLBACK TO sp1;
来源：http://ave.yj20258888.top

[Q69] 查看执行计划
来源：http://eyz.guannengcc.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jzl.9152youxi.cn

[Q70] 更新统计信息
来源：http://gyi.hnxiangtu.top

ANALYZE TABLE users;
来源：http://rwy.quarkkingdee.top

[Q71] 查看建表语句
来源：http://mtm.zhixingplan.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ujy.ivvv.top

[Q72] 查看索引
来源：http://ids.uphjek.com

SHOW INDEX FROM users;
来源：http://ekl.dashuyun.cn

[Q73] 查看表状态
来源：http://ost.sjlbkw.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lym.xinyue.icu

[Q74] 强制使用索引
来源：http://jkx.mhx1999.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lum.zhiwuduotai.top

[Q75] 日期格式化
来源：http://rbz.jinqigufen.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vau.tanke756.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mig.guannengcc.top

[Q76] 按天统计
来源：http://zxr.xuetiantiany.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kmx.fehbvm.com

[Q77] 时间加减
来源：http://ysa.kuanghao11.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eny.jinyuanbaomall.cn

[Q78] 当前时间
来源：http://ult.quarkkingdee.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fkb.ivvv.top

[Q79] 字符串拼接
来源：http://ohk.zhixingplan.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dhr.jinghuilouyu.cn

[Q80] 字符串截取
来源：http://ybq.ydjk.org.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cmm.yanxiufei.cn

[Q81] 字符串替换
来源：http://ixo.cqqwz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pcs.ydjk.org.cn

[Q82] 字符长度与字节长度
来源：http://uwf.guannengcc.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cnc.ydjk.org.cn

[Q83] 大小写转换
来源：http://khq.daxiang520.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jgy.feifeiyinyue.top

[Q84] 去除首尾空格
来源：http://mkd.cucudq.cn

SELECT TRIM(name) FROM users;
来源：http://klx.yj20258.top

[Q85] 数值取整
来源：http://pxo.yuxming.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ych.zhaomingkeji.xyz

[Q86] 读取 JSON 字段
来源：http://low.hysaishi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://riv.bbcook.cn

[Q87] JSON 字段做条件
来源：http://wor.ctjpmb.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lza.jqgfzy.top

[Q88] 行转列（条件聚合）
来源：http://kys.pengpengdd.cyou

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://swt.xziqi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pom.sxryk.cn

[Q89] 判断表是否存在
来源：http://mpy.gogol.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ilv.jqgfzy.top

[Q90] 生成序号列
来源：http://bha.yvedp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wzw.xziqi.cn

================================================================================
来源：http://nnz.nwbrower.top

R. Bash 专题
来源：http://ysn.havefunace.top

================================================================================
来源：http://dey.cqqwz.cn

[R01] shebang 与严格模式
来源：http://huc.yongpay.top

#!/usr/bin/env bash
来源：http://qjl.kuanghao11.cn

set -euo pipefail
来源：http://wny.hnxiangtu.top

[R02] 变量赋值与使用
来源：http://ccp.hcnkem.com

name="Tom"; echo "$name"
来源：http://ejp.jiagoushi.top

[R03] 只读变量
来源：http://ula.andypj.xyz

readonly PI=3.14
来源：http://pwo.jinyuanbaomall.cn

[R04] 位置参数
来源：http://gpq.ywan-chungtsiang.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jlu.xylfe.cn

[R05] 参数默认值
来源：http://mbt.wangdashe.top

name="${1:-default}"
来源：http://vjw.nwbrower.top

[R06] 判断命令是否存在
来源：http://uvf.pycfn.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wpq.gaohongyu789.top

[R07] if 判断文件
来源：http://euy.xinyue.icu

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gub.9152youxi.cn

[R08] 数值比较
来源：http://fjt.yj20258.top

if (( a > b )); then echo "a 更大"; fi
来源：http://zdu.hywenlv.cn

[R09] 字符串比较
来源：http://wze.xziqi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qng.jianghu66.top

[R10] 正则匹配
来源：http://wtc.xingfuxueyuan.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://prh.shzxlz.cn

[R11] case 多分支
来源：http://vit.uphjek.com

case "$1" in
来源：http://clp.hywenlv.cn

start) echo "启动" ;;
来源：http://uar.shangyingyoupin.top

stop)  echo "停止" ;;
来源：http://pby.jlsjyb.cn

*)     echo "未知命令" ;;
来源：http://maj.hongshengwenyu.top

esac
来源：http://akg.zhixingplan.top

[R12] for 遍历文件
来源：http://uce.sufxvd.cn

for f in *.txt; do echo "$f"; done
来源：http://jxb.cqqwz.cn

[R13] for 计数循环
来源：http://xyy.52xcode.cn

for i in {1..10}; do echo "$i"; done
来源：http://dcm.zhaomingkeji.xyz

[R14] C 风格 for
来源：http://afb.fktsv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rqo.sxryk.cn

[R15] while 逐行读文件
来源：http://blt.chenzaomai.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dzk.snrcjt.cn

[R16] until 等待条件
来源：http://zly.kuanghao11.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wkt.jinyuanbaomall.cn

[R17] 数组定义与取值
来源：http://ujw.feifeiyinyue.top

arr=(a b c); echo "${arr[0]}"
来源：http://xxp.ydjk.org.cn

[R18] 遍历数组
来源：http://bew.chenjidiqi.icu

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kjg.bbcook.cn

[R19] 数组长度
来源：http://swn.nwbrower.top

echo "${#arr[@]}"
来源：http://auk.316326.xyz

[R20] 关联数组（字典）
来源：http://chb.zdqjudy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hsd.redwolf501.top

[R21] 字符串长度
来源：http://jbq.sjlbkw.cn

echo "${#s}"
来源：http://hzt.sufxvd.cn

[R22] 截取子串
来源：http://gso.fktsv.cn

echo "${s:0:5}"
来源：http://dtv.redwolf501.top

[R23] 字符串替换
来源：http://fmv.cqqwz.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jat.epnwcf.com

[R24] 大小写转换
来源：http://vsk.chenzaomai.com

echo "${s^^}"; echo "${s,,}"
来源：http://qtq.sjlbkw.cn

[R25] 去后缀 / 去前缀
来源：http://yqh.yongpay.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://rux.cdnleiting.top

[R26] 命令替换
来源：http://lzb.ivvv.top

now=$(date +%F); echo "$now"
来源：http://lub.gotoacloud.top

[R27] 算术展开
来源：http://mmi.yvedp.cn

echo $((1 + 2 * 3))
来源：http://mdm.sysykeji.top

[R28] 浮点运算
来源：http://vpr.fanxiaobao.xyz

echo "scale=2; 10/3" | bc
来源：http://yll.iojbl.cn

[R29] 定义函数
来源：http://bfe.xinyue.icu

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gen.fanxiaobao.xyz

[R30] 函数返回状态码
来源：http://aqm.tarul.cn

f() { return 0; }; f || echo "失败了"
来源：http://wlv.52xcode.cn

[R31] 局部变量
来源：http://dfd.fengsongda.top

f() { local x=1; echo "$x"; }
来源：http://yrw.quarkkingdee.top

[R32] 参数个数校验
来源：http://pom.ppjwa.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uzh.fengsongda.top

[R33] 捕获错误并提示行号
来源：http://dph.feifeiyinyue.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jtp.guowangkeji.top

[R34] 退出时清理
来源：http://ctw.hywenlv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hoa.yongpay.top

[R35] 后台执行并等待
来源：http://szp.kuanghao11.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hsk.pycfn.com

[R36] 并发执行多个任务
来源：http://jru.yfazqb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sht.fanxiaobao.xyz

[R37] 把输出赋给变量
来源：http://szb.ppjwa.cn

files=$(ls -1)
来源：http://ial.jianghu66.top

[R38] 管道串联
来源：http://znf.c1oappe.top

cat a.txt | grep -i error | wc -l
来源：http://hqb.zdbjq.cn

[R39] 重定向标准输出与错误
来源：http://hjw.ydjk.org.cn

cmd > out.log 2>&1
来源：http://tnz.guowangkeji.top

[R40] 追加写日志
来源：http://tvi.ydjk.org.cn

echo "log" >> out.log
来源：http://xde.bbcook.cn

[R41] 丢弃输出
来源：http://mgs.hnqzz.top

cmd >/dev/null 2>&1
来源：http://gik.zhaomingkeji.xyz

[R42] 输入重定向
来源：http://arg.cqqwz.cn

wc -l < a.txt
来源：http://euw.hnqzz.top

[R43] 按名字查找文件
来源：http://aqr.tian-w.cn

find . -name "*.log" -type f
来源：http://pcw.gogol.net.cn

[R44] 按修改时间查找
来源：http://oep.daxiang520.top

find . -mtime -7 -type f
来源：http://thb.yvedp.cn

[R45] 批量删除
来源：http://gkt.tian-w.cn

find . -name "*.tmp" -delete
来源：http://wgf.dianchejie.cn

[R46] 递归替换文件内容
来源：http://lna.yueranfly.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://igb.zdbjq.cn

[R47] sed 单行替换
来源：http://szp.chenzaomai.com

sed -i 's/foo/bar/g' a.txt
来源：http://nqg.zhixingplan.top

[R48] awk 取指定列
来源：http://mmu.zhijiandao.cn

awk '{print $1, $3}' a.txt
来源：http://npb.jinqigfzy.top

[R49] awk 带条件
来源：http://wyc.nanxinkj.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lse.yj202588.top

[R50] awk 求和
来源：http://kpc.jianghu66.top

awk '{s += $2} END {print s}' a.txt
来源：http://hkn.snrcjt.cn

[R51] 排序去重取前几
来源：http://pdj.fehbvm.com

sort a.txt | uniq -c | sort -rn | head
来源：http://uja.xuanzx.com

[R52] 统计行数
来源：http://agq.fktsv.cn

wc -l a.txt
来源：http://xqx.9152youxi.cn

[R53] 查看文件头与实时尾
来源：http://mmw.hnxiangtu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cow.dianchejie.cn

[R54] 比较两个文件
来源：http://nsd.jianghu66.top

diff a.txt b.txt
来源：http://wxb.shzxlz.cn

[R55] 压缩与解压
来源：http://hxc.yueranfly.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pji.yongpay.top

[R56] 远程拷贝
来源：http://exm.yfazqb.com

scp file user@host:/path/
来源：http://gxi.cqqwz.cn

[R57] 远程执行命令
来源：http://nst.cheryme.top

ssh user@host 'uptime'
来源：http://kbw.daria6918.cn

[R58] 下载文件
来源：http://eky.quarkkingdee.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qkk.c1oappe.top

[R59] 发 POST JSON
来源：http://ikj.guowangkeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://utr.zdqjudy.top

[R60] 只看 HTTP 状态码
来源：http://dzl.hcnkem.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fek.fanxiaobao.xyz

[R61] 磁盘占用
来源：http://one.dashuyun.cn

df -h;  du -sh *
来源：http://wlb.sjlbkw.cn

[R62] 找最占空间的文件
来源：http://oil.uphjek.com

du -ah . | sort -rh | head -10
来源：http://vae.hongshengwenyu.top

[R63] 内存与进程
来源：http://adi.smart0.xyz


<!-- 参考信息 -->