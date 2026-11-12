代发 wailian999

SELECT * FROM users;
来源：http://pyq.c1oappe.top

[Q16] 查询指定列
来源：http://zth.chenzaomai.com

SELECT id, name FROM users;
来源：http://oel.shanyushiyangkeji.top

[Q17] 条件查询
来源：http://hpc.birdmap.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ehe.yangfankeji.com

[Q18] 模糊匹配
来源：http://nyd.yuanzhike.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oxs.zhiwuduotai.top

[Q19] 范围查询
来源：http://jth.sufxvd.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hqu.c1oappe.top

[Q20] IN 列表
来源：http://xpt.sweek.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://juu.hammf.cn

[Q21] 空值判断
来源：http://bat.zhongyouzk.top

SELECT * FROM users WHERE email IS NULL;
来源：http://vhd.cqqwz.cn

[Q22] 排序
来源：http://wzk.yvedp.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wpf.mhx1999.top

[Q23] 分页
来源：http://atr.haohaochexian.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xow.mhx1999.top

[Q24] 去重
来源：http://nuw.jlsjyb.cn

SELECT DISTINCT city FROM users;
来源：http://zks.guannengcc.top

[Q25] 只取前 N 条
来源：http://pga.jiagoushi.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ing.ywan-chungtsiang.top

[Q26] 计数
来源：http://fti.cdnleiting.top

SELECT COUNT(*) FROM users;
来源：http://jep.yueranfly.top

[Q27] 条件计数
来源：http://hyy.feifeiyinyue.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yqa.hnxiangtu.top

[Q28] 求和与平均
来源：http://mve.ppjwa.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tdy.aizwys.cn

[Q29] 最大最小值
来源：http://ihk.ctjpmb.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://ufg.chenjidiqi.icu

[Q30] 分组统计
来源：http://hod.bbcook.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rnc.yj202588.top

[Q31] 分组后过滤
来源：http://nbd.fehbvm.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://atc.ybcxt.top

[Q32] 分组拼接字符串
来源：http://omw.xziqi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zmu.cheryme.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ehy.yonumen.top

[Q33] 多列分组
来源：http://hcf.yueranfly.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yab.hysaishi.cn

[Q34] 每组取第一条
来源：http://qsr.cheryme.top

SELECT * FROM (
来源：http://vuu.hcnkem.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vpw.jyoumei.cn

) t WHERE rn = 1;
来源：http://txm.yanxiufei.cn

[Q35] 内连接
来源：http://sdu.guowangkeji.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zbe.hcnkem.com

[Q36] 左连接
来源：http://ypt.daxiang520.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vuj.zhongyouzk.top

[Q37] 右连接
来源：http://xts.316326.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mqj.wangdashe.top

[Q38] 全外连接（PostgreSQL）
来源：http://fwf.meibo888.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://eal.fzhhl.top

[Q39] 自连接（查上下级）
来源：http://nqm.haohaochexian.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://usy.xuetiantiany.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qkz.hongshengwenyu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://hcx.zhaomingkeji.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yzg.bbcook.cn

[Q41] 多表连接
来源：http://ils.52xcode.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://juo.pycfn.com

JOIN users u ON u.id = o.user_id
来源：http://tcc.chenjidiqi.icu

JOIN products p ON p.id = o.product_id;
来源：http://jxa.epnwcf.com

[Q42] 连接条件附加过滤
来源：http://joq.iojbl.cn

SELECT u.name, o.amount FROM users u
来源：http://qwj.52xcode.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dya.iojbl.cn

[Q43] 标量子查询
来源：http://owa.chenlongwang.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://syy.c1oappe.top

[Q44] IN 子查询
来源：http://nuq.smart0.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wbn.chenlongwang.top

[Q45] EXISTS 判断存在
来源：http://icu.andypj.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bxy.jiagoushi.top

[Q46] NOT EXISTS 判断不存在
来源：http://dab.hnxiangtu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mak.snrcjt.cn

[Q47] 与平均值比较
来源：http://mzk.yuxming.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wol.yangfankeji.com

[Q48] CTE 公用表表达式
来源：http://jqr.uphjek.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vce.xziqi.cn

SELECT * FROM t WHERE c > 5;
来源：http://qru.xuetiantiany.cn

[Q49] 更新单行
来源：http://nql.zhengqikj.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://psk.havefunace.top

[Q50] 批量更新
来源：http://arg.jiagoushi.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lke.hysaishi.cn

[Q51] 用子查询更新
来源：http://vcb.dashuyun.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ljv.tianlin.xyz

[Q52] 删除指定行
来源：http://gmn.ywan-chungtsiang.top

DELETE FROM users WHERE id = 10;
来源：http://wvo.cheryme.top

[Q53] 按条件删除
来源：http://idr.yj20258888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wkn.smart0.xyz

[Q54] 清空表
来源：http://vfc.wangdashe.top

TRUNCATE TABLE logs;
来源：http://fqd.tianlin.xyz

[Q55] 排名（并列占位）
来源：http://hdq.hesvh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ctr.bbcook.cn

[Q56] 密集排名（并列不占位）
来源：http://bak.0kj1m.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mhh.haohaochexian.top

[Q57] 行号
来源：http://mfa.mhx1999.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hqb.fehbvm.com

[Q58] 累计求和
来源：http://mzd.smart0.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://exf.sxryk.cn

[Q59] 分组内累计
来源：http://ray.cqqwz.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jnq.chenzaomai.com

[Q60] 取上一行 / 下一行
来源：http://xdi.52xcode.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ver.hnxiangtu.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ftm.dashuyun.cn

[Q61] 移动平均
来源：http://jow.xuetiantiany.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ewm.ivvv.top

[Q62] 分组占比
来源：http://wyc.gaohongyu789.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vqa.cashguo.top

[Q63] 开启事务
来源：http://gzt.sysykeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://lpd.zhoulong.xyz

[Q64] 提交事务
来源：http://liv.fengsongda.top

COMMIT;
来源：http://nfu.zhixingplan.top

[Q65] 回滚事务
来源：http://ivy.snrcjt.cn

ROLLBACK;
来源：http://cck.bjfxy.top

[Q66] 行锁查询
来源：http://mtz.feifeiyinyue.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://azf.fanxiaobao.xyz

[Q67] 设置隔离级别
来源：http://iiy.smart0.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ple.tarul.cn

[Q68] 保存点
来源：http://wio.hywenlv.cn

SAVEPOINT sp1;
来源：http://cpq.sxryk.cn

ROLLBACK TO sp1;
来源：http://rgr.ehwqpu.com

[Q69] 查看执行计划
来源：http://dqe.nanxinkj.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jsb.shanyushiyangkeji.top

[Q70] 更新统计信息
来源：http://gpc.zhixingplan.top

ANALYZE TABLE users;
来源：http://gov.hnqzz.top

[Q71] 查看建表语句
来源：http://yhx.mhx1999.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bzh.dianchejie.cn

[Q72] 查看索引
来源：http://mbq.aizwys.cn

SHOW INDEX FROM users;
来源：http://hnt.tian-w.cn

[Q73] 查看表状态
来源：http://mck.cashguo.top

SHOW TABLE STATUS LIKE 'users';
来源：http://iap.zhixingplan.top

[Q74] 强制使用索引
来源：http://prf.ivvv.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ahd.jqgufenzy.top

[Q75] 日期格式化
来源：http://iud.feifeiyinyue.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pbu.wangdashe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sni.cheryme.top

[Q76] 按天统计
来源：http://adh.cdnleiting.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gdr.sjlbkw.cn

[Q77] 时间加减
来源：http://dap.chenzaomai.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kep.tarul.cn

[Q78] 当前时间
来源：http://cie.zdbjq.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://eop.yonumen.top

[Q79] 字符串拼接
来源：http://xit.andypj.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://def.fengsongda.top

[Q80] 字符串截取
来源：http://doz.jinyuanbaomall.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://byz.cdnleiting.top

[Q81] 字符串替换
来源：http://osg.ivvv.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xyj.0kj1m.cn

[Q82] 字符长度与字节长度
来源：http://wll.hesvh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wqt.iojbl.cn

[Q83] 大小写转换
来源：http://kve.epnwcf.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sxf.epnwcf.com

[Q84] 去除首尾空格
来源：http://hue.xuetiantiany.cn

SELECT TRIM(name) FROM users;
来源：http://rfs.jyoumei.cn

[Q85] 数值取整
来源：http://rpe.sjlbkw.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tni.daria6918.cn

[Q86] 读取 JSON 字段
来源：http://lji.nwbrower.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://shj.epnwcf.com

[Q87] JSON 字段做条件
来源：http://gbs.shanyushiyangtech.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bjb.meibo888.top

[Q88] 行转列（条件聚合）
来源：http://iam.ehwqpu.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blr.tarul.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vwe.ivvv.top

[Q89] 判断表是否存在
来源：http://rjq.fanxiaobao.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://squ.fzhhl.top

[Q90] 生成序号列
来源：http://xkg.shzxlz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vru.mhx1999.top

================================================================================
来源：http://pef.yuxming.cn

R. Bash 专题
来源：http://llx.chenzaomai.com

================================================================================
来源：http://hsx.birdmap.top

[R01] shebang 与严格模式
来源：http://uhf.dashuyun.cn

#!/usr/bin/env bash
来源：http://jiy.jqgfzy.top

set -euo pipefail
来源：http://gzv.svipenyu.cn

[R02] 变量赋值与使用
来源：http://wxl.zdqjudy.top

name="Tom"; echo "$name"
来源：http://xos.0kj1m.cn

[R03] 只读变量
来源：http://gii.c1oappe.top

readonly PI=3.14
来源：http://auc.nwbrower.top

[R04] 位置参数
来源：http://zzr.cashguo.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ldl.hcnkem.com

[R05] 参数默认值
来源：http://nrr.zhiwuduotai.top

name="${1:-default}"
来源：http://flq.hywenlv.cn

[R06] 判断命令是否存在
来源：http://bjd.smart0.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mci.yonumen.top

[R07] if 判断文件
来源：http://unf.fehbvm.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://twg.chenlongwang.top

[R08] 数值比较
来源：http://rjr.cqqwz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bef.jinqigufen.top

[R09] 字符串比较
来源：http://qxe.yfazqb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tyj.nanxuanxn.top

[R10] 正则匹配
来源：http://eca.jlsjyb.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wmx.hnqzz.top

[R11] case 多分支
来源：http://wso.hammf.cn

case "$1" in
来源：http://iiw.hammf.cn

start) echo "启动" ;;
来源：http://ebh.andypj.xyz

stop)  echo "停止" ;;
来源：http://gft.jinyuanbaomall.cn

*)     echo "未知命令" ;;
来源：http://cqx.xuanzx.com

esac
来源：http://vox.9152youxi.cn

[R12] for 遍历文件
来源：http://asv.guowangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://yym.birdmap.top

[R13] for 计数循环
来源：http://jns.yj20258.top

for i in {1..10}; do echo "$i"; done
来源：http://dzt.zdbjq.cn

[R14] C 风格 for
来源：http://gan.dashuyun.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dvu.zhengqikj.top

[R15] while 逐行读文件
来源：http://bqr.xingfuxueyuan.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vgs.shanyushiyangkeji.top

[R16] until 等待条件
来源：http://rot.iojbl.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xng.birdmap.top

[R17] 数组定义与取值
来源：http://cxg.epnwcf.com

arr=(a b c); echo "${arr[0]}"
来源：http://zag.sjlbkw.cn

[R18] 遍历数组
来源：http://mjy.yongpay.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gxf.guowangkeji.top

[R19] 数组长度
来源：http://ckb.fehbvm.com

echo "${#arr[@]}"
来源：http://qmg.ehwqpu.com

[R20] 关联数组（字典）
来源：http://pxf.zdbjq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tbk.hammf.cn

[R21] 字符串长度
来源：http://mxz.hywenlv.cn

echo "${#s}"
来源：http://mlf.uphjek.com

[R22] 截取子串
来源：http://rcs.sjlbkw.cn

echo "${s:0:5}"
来源：http://lyv.jinghuilouyu.cn

[R23] 字符串替换
来源：http://csi.zhongyouzk.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ljt.c1oappe.top

[R24] 大小写转换
来源：http://frj.jinyuanbaomall.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vfq.guannengcc.top

[R25] 去后缀 / 去前缀
来源：http://qxl.sxryk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mee.hammf.cn

[R26] 命令替换
来源：http://cja.ppjwa.cn

now=$(date +%F); echo "$now"
来源：http://ayt.quarkkingdee.top

[R27] 算术展开
来源：http://xcm.hammf.cn

echo $((1 + 2 * 3))
来源：http://daw.yj20258888.top

[R28] 浮点运算
来源：http://odu.c1oappe.top

echo "scale=2; 10/3" | bc
来源：http://szq.zhijiandao.cn

[R29] 定义函数
来源：http://qbd.hongshengwenyu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gvg.zhoulong.xyz

[R30] 函数返回状态码
来源：http://qsp.zhengqikj.top

f() { return 0; }; f || echo "失败了"
来源：http://pbg.zhixingplan.top

[R31] 局部变量
来源：http://irs.tanke756.top

f() { local x=1; echo "$x"; }
来源：http://yfr.wangdashe.top

[R32] 参数个数校验
来源：http://gtu.kuanghao11.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://axt.kuanghao11.cn

[R33] 捕获错误并提示行号
来源：http://ncm.epnwcf.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wwt.chenzaomai.com

[R34] 退出时清理
来源：http://zsl.shuidangran.top

trap 'rm -f "$tmp"' EXIT
来源：http://nen.redwolf501.top

[R35] 后台执行并等待
来源：http://jsj.jiagoushi.top

sleep 5 & pid=$!; wait "$pid"
来源：http://qnq.yuxming.cn

[R36] 并发执行多个任务
来源：http://hyn.mhx1999.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://chl.tianlin.xyz

[R37] 把输出赋给变量
来源：http://yax.yj20258.top

files=$(ls -1)
来源：http://mla.redwolf501.top

[R38] 管道串联
来源：http://emz.cdnleiting.top

cat a.txt | grep -i error | wc -l
来源：http://yjx.redwolf501.top

[R39] 重定向标准输出与错误
来源：http://hjg.chenlongwang.top

cmd > out.log 2>&1
来源：http://wqg.tian-w.cn

[R40] 追加写日志
来源：http://mxi.redwolf501.top

echo "log" >> out.log
来源：http://koe.fengsongda.top

[R41] 丢弃输出
来源：http://vkw.chenlongwang.top

cmd >/dev/null 2>&1
来源：http://ogx.fanxiaobao.xyz

[R42] 输入重定向
来源：http://hri.cucudq.cn

wc -l < a.txt
来源：http://ozy.gaohongyu789.top

[R43] 按名字查找文件
来源：http://cmo.ppjwa.cn

find . -name "*.log" -type f
来源：http://rcp.aibaodan.cn

[R44] 按修改时间查找
来源：http://gaj.gaohongyu789.top

find . -mtime -7 -type f
来源：http://wqh.zhaomingkeji.xyz

[R45] 批量删除
来源：http://mfn.cheryme.top

find . -name "*.tmp" -delete
来源：http://ezc.yj202588.top

[R46] 递归替换文件内容
来源：http://kvk.aizwys.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://agv.sxryk.cn

[R47] sed 单行替换
来源：http://umx.zdqjudy.top

sed -i 's/foo/bar/g' a.txt
来源：http://swd.haohaochexian.top

[R48] awk 取指定列
来源：http://vcf.yvedp.cn

awk '{print $1, $3}' a.txt
来源：http://dlw.zhoulong.xyz

[R49] awk 带条件
来源：http://nci.feifeiyinyue.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://azx.cheryme.top

[R50] awk 求和
来源：http://qcg.xuetiantiany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gqx.fehbvm.com

[R51] 排序去重取前几
来源：http://wwu.yj20258.top

sort a.txt | uniq -c | sort -rn | head
来源：http://hil.guowangkeji.top

[R52] 统计行数
来源：http://fxd.mhx1999.top

wc -l a.txt
来源：http://djo.ehwqpu.com

[R53] 查看文件头与实时尾
来源：http://cqn.jinqigfzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hde.wangdashe.top

[R54] 比较两个文件
来源：http://eqj.tianlin.xyz

diff a.txt b.txt
来源：http://pbk.nwbrower.top

[R55] 压缩与解压
来源：http://yyc.vehdjk.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mpp.quarkkingdee.top

[R56] 远程拷贝
来源：http://khc.smart0.xyz

scp file user@host:/path/
来源：http://nst.zycfv.cn

[R57] 远程执行命令
来源：http://odo.yvedp.cn

ssh user@host 'uptime'
来源：http://wvb.zhengqikj.top

[R58] 下载文件
来源：http://qhf.nanxinkj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gjv.fengsongda.top

[R59] 发 POST JSON
来源：http://wzq.yvedp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dsu.c1oappe.top

[R60] 只看 HTTP 状态码
来源：http://fyw.tianlin.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xkx.dashuyun.cn

[R61] 磁盘占用
来源：http://aow.tarul.cn

df -h;  du -sh *
来源：http://xgw.sufxvd.cn

[R62] 找最占空间的文件
来源：http://sxe.shuidangran.top

du -ah . | sort -rh | head -10
来源：http://mcf.aibaodan.cn

[R63] 内存与进程
来源：http://jvh.yj20258.top

free -h;  ps aux | grep nginx
来源：http://gud.hammf.cn

[R64] 结束进程
来源：http://ani.fehbvm.com

kill -9 $(pgrep -f app.py)
来源：http://fcb.nanxuanxn.top

[R65] 查看端口占用
来源：http://luv.jqgufenzy.top


<!-- 参考信息 -->