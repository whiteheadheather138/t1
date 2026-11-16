代发 wailian999

SELECT * FROM users;
来源：http://ice.jyoumei.cn

[Q16] 查询指定列
来源：http://zbv.tanke756.top

SELECT id, name FROM users;
来源：http://ufe.yangfankeji.com

[Q17] 条件查询
来源：http://nvk.shzxlz.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qhp.daxiang520.top

[Q18] 模糊匹配
来源：http://mdl.c1oappe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fyy.nanxinkj.top

[Q19] 范围查询
来源：http://oeb.feifeiyinyue.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ikm.birdmap.top

[Q20] IN 列表
来源：http://zbr.meibo888.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kqz.hysaishi.cn

[Q21] 空值判断
来源：http://zaj.dianchejie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gcp.yvedp.cn

[Q22] 排序
来源：http://wcq.jqgufenzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jau.sjlbkw.cn

[Q23] 分页
来源：http://vdw.zdqjudy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zav.yonumen.top

[Q24] 去重
来源：http://jti.meibo888.top

SELECT DISTINCT city FROM users;
来源：http://dps.yonumen.top

[Q25] 只取前 N 条
来源：http://qjp.zhongyouzk.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kyu.tian-w.cn

[Q26] 计数
来源：http://olq.jqgfzy.top

SELECT COUNT(*) FROM users;
来源：http://mbb.cucudq.cn

[Q27] 条件计数
来源：http://pfw.hnxiangtu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cdb.yuxming.cn

[Q28] 求和与平均
来源：http://zaa.yangfankeji.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pag.chenzaomai.com

[Q29] 最大最小值
来源：http://mpp.yj202588.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://dxg.gogol.net.cn

[Q30] 分组统计
来源：http://qyr.zhongyouzk.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://iht.zhoulong.xyz

[Q31] 分组后过滤
来源：http://fqm.vehdjk.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yok.yuxming.cn

[Q32] 分组拼接字符串
来源：http://xzw.aibaodan.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://que.hongshengwenyu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lzu.zhijiandao.cn

[Q33] 多列分组
来源：http://xyx.daria6918.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hjj.yfazqb.com

[Q34] 每组取第一条
来源：http://oac.haohaochexian.top

SELECT * FROM (
来源：http://moc.hfpthk.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sxc.tian-w.cn

) t WHERE rn = 1;
来源：http://xkt.0kj1m.cn

[Q35] 内连接
来源：http://vsx.hesvh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uai.xuetiantiany.cn

[Q36] 左连接
来源：http://sxr.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mau.smart0.xyz

[Q37] 右连接
来源：http://phw.zhongyouzk.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qdt.yj20258.top

[Q38] 全外连接（PostgreSQL）
来源：http://nxu.xinyue.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lyc.jyoumei.cn

[Q39] 自连接（查上下级）
来源：http://cnu.zhengqikj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://afj.hesvh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://czm.yj20258888.top

[Q40] 交叉连接（笛卡尔积）
来源：http://nwq.cashguo.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qgv.snrcjt.cn

[Q41] 多表连接
来源：http://bgi.tanke756.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ehm.ivvv.top

JOIN users u ON u.id = o.user_id
来源：http://ypg.sufxvd.cn

JOIN products p ON p.id = o.product_id;
来源：http://aef.daria6918.cn

[Q42] 连接条件附加过滤
来源：http://ica.ppjwa.cn

SELECT u.name, o.amount FROM users u
来源：http://xtb.sxryk.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lfj.xuetiantiany.cn

[Q43] 标量子查询
来源：http://ygt.tarul.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://voc.fktsv.cn

[Q44] IN 子查询
来源：http://djt.jqgufenzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://inh.zdbjq.cn

[Q45] EXISTS 判断存在
来源：http://sqd.uphjek.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ivb.svipenyu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ecp.shanyushiyangtech.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kso.hnxiangtu.top

[Q47] 与平均值比较
来源：http://xzy.hcnkem.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ljh.ywan-chungtsiang.top

[Q48] CTE 公用表表达式
来源：http://mbe.chenzaomai.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ajg.haohaochexian.top

SELECT * FROM t WHERE c > 5;
来源：http://brr.hnqzz.top

[Q49] 更新单行
来源：http://mcl.52xcode.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nyz.zhijiandao.cn

[Q50] 批量更新
来源：http://xbh.yongpay.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yua.fzhhl.top

[Q51] 用子查询更新
来源：http://byt.chenjidiqi.icu

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://duv.iojbl.cn

[Q52] 删除指定行
来源：http://fug.chenlongwang.top

DELETE FROM users WHERE id = 10;
来源：http://npf.redwolf501.top

[Q53] 按条件删除
来源：http://qyb.jyoumei.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uhs.zhixingplan.top

[Q54] 清空表
来源：http://ndx.jinqigfzy.top

TRUNCATE TABLE logs;
来源：http://zsn.dashuyun.cn

[Q55] 排名（并列占位）
来源：http://sac.quarkkingdee.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://izx.tian-w.cn

[Q56] 密集排名（并列不占位）
来源：http://wxw.shanyushiyangkeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uki.yvedp.cn

[Q57] 行号
来源：http://nla.svipenyu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jkv.jqgufenzy.top

[Q58] 累计求和
来源：http://lvn.yvedp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jfk.epnwcf.com

[Q59] 分组内累计
来源：http://ryc.cdnleiting.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hhz.gogol.net.cn

[Q60] 取上一行 / 下一行
来源：http://rqx.ivvv.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ken.ctjpmb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://brv.yvedp.cn

[Q61] 移动平均
来源：http://zba.chenzaomai.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://veg.zhixingplan.top

[Q62] 分组占比
来源：http://tnb.meibo888.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mlb.yangfankeji.com

[Q63] 开启事务
来源：http://fpy.xuetiantiany.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ahc.mhx1999.top

[Q64] 提交事务
来源：http://uvy.fktsv.cn

COMMIT;
来源：http://koa.zycfv.cn

[Q65] 回滚事务
来源：http://pgq.jinghuilouyu.cn

ROLLBACK;
来源：http://tvw.jiagoushi.top

[Q66] 行锁查询
来源：http://xcu.ivvv.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lda.ywan-chungtsiang.top

[Q67] 设置隔离级别
来源：http://bhk.uphjek.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uhg.zhaomingkeji.xyz

[Q68] 保存点
来源：http://zmu.xylfe.cn

SAVEPOINT sp1;
来源：http://sny.cdnleiting.top

ROLLBACK TO sp1;
来源：http://wep.andypj.xyz

[Q69] 查看执行计划
来源：http://bko.vqdsnc.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fce.aibaodan.cn

[Q70] 更新统计信息
来源：http://cpg.fehbvm.com

ANALYZE TABLE users;
来源：http://blr.aibaodan.cn

[Q71] 查看建表语句
来源：http://ori.smart0.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eut.guowangkeji.top

[Q72] 查看索引
来源：http://ixr.guannengcc.top

SHOW INDEX FROM users;
来源：http://brw.vqdsnc.cn

[Q73] 查看表状态
来源：http://ahh.gaohongyu789.top

SHOW TABLE STATUS LIKE 'users';
来源：http://bxc.pengpengdd.cyou

[Q74] 强制使用索引
来源：http://myx.hnqzz.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://eej.wangdashe.top

[Q75] 日期格式化
来源：http://zkh.jinghuilouyu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ewj.jlsjyb.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lix.zhongyouzk.top

[Q76] 按天统计
来源：http://qav.ivvv.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sjo.jinqigfzy.top

[Q77] 时间加减
来源：http://bhd.svipenyu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ldb.jlsjyb.cn

[Q78] 当前时间
来源：http://imf.bjfxy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://usz.xinyue.icu

[Q79] 字符串拼接
来源：http://jve.jinqigufen.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xfj.bjfxy.top

[Q80] 字符串截取
来源：http://vtt.fanxiaobao.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yvc.birdmap.top

[Q81] 字符串替换
来源：http://nyu.yuanzhike.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zdr.hammf.cn

[Q82] 字符长度与字节长度
来源：http://dfq.hnqzz.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rhz.shanyushiyangkeji.top

[Q83] 大小写转换
来源：http://owp.hongshengwenyu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rmx.ppjwa.cn

[Q84] 去除首尾空格
来源：http://zhs.c1oappe.top

SELECT TRIM(name) FROM users;
来源：http://utt.jinghuilouyu.cn

[Q85] 数值取整
来源：http://ivu.vqdsnc.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xbo.fehbvm.com

[Q86] 读取 JSON 字段
来源：http://ojt.xingfuxueyuan.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://opp.ppjwa.cn

[Q87] JSON 字段做条件
来源：http://fpk.vehdjk.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fbh.ivvv.top

[Q88] 行转列（条件聚合）
来源：http://tew.sjlbkw.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uil.ppjwa.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fpp.sxryk.cn

[Q89] 判断表是否存在
来源：http://gat.uphjek.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://aui.tianlin.xyz

[Q90] 生成序号列
来源：http://piw.jinghuilouyu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wmg.epnwcf.com

================================================================================
来源：http://xds.tianlin.xyz

R. Bash 专题
来源：http://zyu.cucudq.cn

================================================================================
来源：http://hed.pycfn.com

[R01] shebang 与严格模式
来源：http://qcd.ppjwa.cn

#!/usr/bin/env bash
来源：http://wkz.guannengcc.top

set -euo pipefail
来源：http://pgx.sweek.top

[R02] 变量赋值与使用
来源：http://wfr.hfpthk.cn

name="Tom"; echo "$name"
来源：http://ybm.fktsv.cn

[R03] 只读变量
来源：http://cwt.nwbrower.top

readonly PI=3.14
来源：http://lnp.hesvh.cn

[R04] 位置参数
来源：http://ilm.nanxuanxn.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xdy.zycfv.cn

[R05] 参数默认值
来源：http://atl.ydzc1.top

name="${1:-default}"
来源：http://fim.pycfn.com

[R06] 判断命令是否存在
来源：http://mru.hfpthk.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xle.gzhubu.top

[R07] if 判断文件
来源：http://pzn.fanxiaobao.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yav.shanyushiyangkeji.top

[R08] 数值比较
来源：http://ioy.svipenyu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kgl.uphjek.com

[R09] 字符串比较
来源：http://brm.jinghuilouyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gjf.shanyushiyangkeji.top

[R10] 正则匹配
来源：http://maw.aizwys.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ffx.yfazqb.com

[R11] case 多分支
来源：http://kjz.meibo888.top

case "$1" in
来源：http://jjy.jyoumei.cn

start) echo "启动" ;;
来源：http://tvz.kuanghao11.cn

stop)  echo "停止" ;;
来源：http://kla.xuanzx.com

*)     echo "未知命令" ;;
来源：http://rtl.cqqwz.cn

esac
来源：http://bzo.haohaochexian.top

[R12] for 遍历文件
来源：http://qka.jinyuanbaomall.cn

for f in *.txt; do echo "$f"; done
来源：http://xko.vehdjk.com

[R13] for 计数循环
来源：http://vcs.yj20258888.top

for i in {1..10}; do echo "$i"; done
来源：http://xgk.yfazqb.com

[R14] C 风格 for
来源：http://muh.zhixingplan.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gze.cashguo.top

[R15] while 逐行读文件
来源：http://lbv.cheryme.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zzv.xuanzx.com

[R16] until 等待条件
来源：http://kpq.yj20258.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nqd.52xcode.cn

[R17] 数组定义与取值
来源：http://qku.svipenyu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oto.sweek.top

[R18] 遍历数组
来源：http://rsb.zhoulong.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lpo.yanxiufei.cn

[R19] 数组长度
来源：http://xaf.yvedp.cn

echo "${#arr[@]}"
来源：http://kqd.gotoacloud.top

[R20] 关联数组（字典）
来源：http://wko.guowangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mrx.nanxuanxn.top

[R21] 字符串长度
来源：http://wof.ydjk.org.cn

echo "${#s}"
来源：http://olh.chenjidiqi.icu

[R22] 截取子串
来源：http://hzw.ppjwa.cn

echo "${s:0:5}"
来源：http://igr.c1oappe.top

[R23] 字符串替换
来源：http://hqm.guowangkeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kak.nwbrower.top

[R24] 大小写转换
来源：http://exq.gaohongyu789.top

echo "${s^^}"; echo "${s,,}"
来源：http://arf.meibo888.top

[R25] 去后缀 / 去前缀
来源：http://uin.ehwqpu.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://muc.tian-w.cn

[R26] 命令替换
来源：http://utw.wangshuangyany.cn

now=$(date +%F); echo "$now"
来源：http://pfy.fzhhl.top

[R27] 算术展开
来源：http://lal.gogol.net.cn

echo $((1 + 2 * 3))
来源：http://bpp.sweek.top

[R28] 浮点运算
来源：http://hnj.haohaochexian.top

echo "scale=2; 10/3" | bc
来源：http://yut.jinqigufen.top

[R29] 定义函数
来源：http://tan.haohaochexian.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://emr.tanke756.top

[R30] 函数返回状态码
来源：http://akw.chenlongwang.top

f() { return 0; }; f || echo "失败了"
来源：http://wod.tarul.cn

[R31] 局部变量
来源：http://ybe.hammf.cn

f() { local x=1; echo "$x"; }
来源：http://opk.dashuyun.cn

[R32] 参数个数校验
来源：http://ohu.ydjk.org.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://amu.sxryk.cn

[R33] 捕获错误并提示行号
来源：http://ucc.zycfv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wnj.sxryk.cn

[R34] 退出时清理
来源：http://qtd.hcnkem.com

trap 'rm -f "$tmp"' EXIT
来源：http://hyz.meibo888.top

[R35] 后台执行并等待
来源：http://ncl.316326.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://hep.cashguo.top

[R36] 并发执行多个任务
来源：http://fak.hnqzz.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gqr.tarul.cn

[R37] 把输出赋给变量
来源：http://kff.0kj1m.cn

files=$(ls -1)
来源：http://kxy.vehdjk.com

[R38] 管道串联
来源：http://opt.hnqzz.top

cat a.txt | grep -i error | wc -l
来源：http://mif.tian-w.cn

[R39] 重定向标准输出与错误
来源：http://amp.sweek.top

cmd > out.log 2>&1
来源：http://ghu.kuanghao11.cn

[R40] 追加写日志
来源：http://pnt.yj20258.top

echo "log" >> out.log
来源：http://jne.yvedp.cn

[R41] 丢弃输出
来源：http://hbe.gaohongyu789.top

cmd >/dev/null 2>&1
来源：http://msf.yongpay.top

[R42] 输入重定向
来源：http://mqs.xziqi.cn

wc -l < a.txt
来源：http://ayp.quarkkingdee.top

[R43] 按名字查找文件
来源：http://aju.chenlongwang.top

find . -name "*.log" -type f
来源：http://lrs.jiagoushi.top

[R44] 按修改时间查找
来源：http://via.shuidangran.top

find . -mtime -7 -type f
来源：http://zmt.9152youxi.cn

[R45] 批量删除
来源：http://mvj.sjlbkw.cn

find . -name "*.tmp" -delete
来源：http://wpz.shzxlz.cn

[R46] 递归替换文件内容
来源：http://cka.yj20258.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mxg.jinqigufen.top

[R47] sed 单行替换
来源：http://yyi.yvedp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dmr.epnwcf.com

[R48] awk 取指定列
来源：http://kuj.sufxvd.cn

awk '{print $1, $3}' a.txt
来源：http://vti.havefunace.top

[R49] awk 带条件
来源：http://rji.52xcode.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nrs.hywenlv.cn

[R50] awk 求和
来源：http://byy.fzhhl.top

awk '{s += $2} END {print s}' a.txt
来源：http://egc.smart0.xyz

[R51] 排序去重取前几
来源：http://gua.jqgufenzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://dvv.feifeiyinyue.top

[R52] 统计行数
来源：http://dbh.shzxlz.cn

wc -l a.txt
来源：http://zfj.iojbl.cn

[R53] 查看文件头与实时尾
来源：http://vsw.tanke756.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pnj.tarul.cn

[R54] 比较两个文件
来源：http://mvu.hesvh.cn

diff a.txt b.txt
来源：http://cqu.316326.xyz

[R55] 压缩与解压
来源：http://uma.sufxvd.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vdz.zdbjq.cn

[R56] 远程拷贝
来源：http://gpg.fengsongda.top

scp file user@host:/path/
来源：http://lfn.gogol.net.cn

[R57] 远程执行命令
来源：http://yzz.shangyingyoupin.top

ssh user@host 'uptime'
来源：http://aei.pengpengdd.cyou

[R58] 下载文件
来源：http://uvk.c1oappe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nal.zdqjudy.top

[R59] 发 POST JSON
来源：http://iza.jinyuanbaomall.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ioc.gzhubu.top

[R60] 只看 HTTP 状态码
来源：http://hbe.yangfankeji.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hmw.tian-w.cn

[R61] 磁盘占用
来源：http://yxi.daria6918.cn

df -h;  du -sh *
来源：http://wzh.zhoulong.xyz

[R62] 找最占空间的文件
来源：http://qjr.jyoumei.cn

du -ah . | sort -rh | head -10
来源：http://avi.yangfankeji.com

[R63] 内存与进程
来源：http://plu.shanyushiyangkeji.top

free -h;  ps aux | grep nginx
来源：http://fxf.gzhubu.top

[R64] 结束进程
来源：http://jhi.ybcxt.top

kill -9 $(pgrep -f app.py)
来源：http://gvf.mhx1999.top

[R65] 查看端口占用
来源：http://lmg.ppjwa.cn


<!-- 参考信息 -->