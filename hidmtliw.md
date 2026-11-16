代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://eep.gzhubu.top

[Q20] IN 列表
来源：http://bik.vqdsnc.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://amr.cheryme.top

[Q21] 空值判断
来源：http://wug.tian-w.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yhj.hnqzz.top

[Q22] 排序
来源：http://uyr.zycfv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qrt.hongshengwenyu.top

[Q23] 分页
来源：http://lvf.feifeiyinyue.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://keb.jinyuanbaomall.cn

[Q24] 去重
来源：http://mby.nanxinkj.top

SELECT DISTINCT city FROM users;
来源：http://igb.gotoacloud.top

[Q25] 只取前 N 条
来源：http://lyf.ehwqpu.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gyp.jinghuilouyu.cn

[Q26] 计数
来源：http://ifl.hysaishi.cn

SELECT COUNT(*) FROM users;
来源：http://cga.zhengqikj.top

[Q27] 条件计数
来源：http://mkn.yj202588.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wby.xylfe.cn

[Q28] 求和与平均
来源：http://ilh.sufxvd.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mqv.feifeiyinyue.top

[Q29] 最大最小值
来源：http://wvf.guowangkeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://bol.xingfuxueyuan.xyz

[Q30] 分组统计
来源：http://dsw.kuanghao11.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tiv.gogol.net.cn

[Q31] 分组后过滤
来源：http://mrq.pycfn.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bse.zdqjudy.top

[Q32] 分组拼接字符串
来源：http://lpg.yj20258.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vlb.gaohongyu789.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://szx.xingfuxueyuan.xyz

[Q33] 多列分组
来源：http://wcr.tanke756.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://neq.ywan-chungtsiang.top

[Q34] 每组取第一条
来源：http://zjl.hammf.cn

SELECT * FROM (
来源：http://mem.wangdashe.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bqw.yanxiufei.cn

) t WHERE rn = 1;
来源：http://xkf.feifeiyinyue.top

[Q35] 内连接
来源：http://bhx.zhongyouzk.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tgy.c1oappe.top

[Q36] 左连接
来源：http://hke.jqgfzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zuo.aizwys.cn

[Q37] 右连接
来源：http://vyu.ywan-chungtsiang.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zvv.pycfn.com

[Q38] 全外连接（PostgreSQL）
来源：http://itb.316326.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vga.shzxlz.cn

[Q39] 自连接（查上下级）
来源：http://qag.c1oappe.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://tsy.tian-w.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rbq.yueranfly.top

[Q40] 交叉连接（笛卡尔积）
来源：http://yvs.ctjpmb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://grv.xinyue.icu

[Q41] 多表连接
来源：http://uxu.hnqzz.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://uxn.cdnleiting.top

JOIN users u ON u.id = o.user_id
来源：http://yxs.hnxiangtu.top

JOIN products p ON p.id = o.product_id;
来源：http://ovb.zhengqikj.top

[Q42] 连接条件附加过滤
来源：http://adx.gzhubu.top

SELECT u.name, o.amount FROM users u
来源：http://adm.snrcjt.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zau.mhx1999.top

[Q43] 标量子查询
来源：http://oxw.feifeiyinyue.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://whp.yvedp.cn

[Q44] IN 子查询
来源：http://kqw.tanke756.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://drb.ywan-chungtsiang.top

[Q45] EXISTS 判断存在
来源：http://ksl.mhx1999.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vxh.yueranfly.top

[Q46] NOT EXISTS 判断不存在
来源：http://dzs.hammf.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nqy.yueranfly.top

[Q47] 与平均值比较
来源：http://cmx.pengpengdd.cyou

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dek.9152youxi.cn

[Q48] CTE 公用表表达式
来源：http://ojx.shuidangran.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uhv.fehbvm.com

SELECT * FROM t WHERE c > 5;
来源：http://fim.shangyingyoupin.top

[Q49] 更新单行
来源：http://gdv.yvedp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nso.c1oappe.top

[Q50] 批量更新
来源：http://pyj.redwolf501.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jxi.andypj.xyz

[Q51] 用子查询更新
来源：http://hyg.hywenlv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zuv.sxryk.cn

[Q52] 删除指定行
来源：http://knt.fzhhl.top

DELETE FROM users WHERE id = 10;
来源：http://rxw.shangyingyoupin.top

[Q53] 按条件删除
来源：http://wty.smart0.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ksv.havefunace.top

[Q54] 清空表
来源：http://oni.xingfuxueyuan.xyz

TRUNCATE TABLE logs;
来源：http://gnf.snrcjt.cn

[Q55] 排名（并列占位）
来源：http://zxt.snrcjt.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ccx.xinyue.icu

[Q56] 密集排名（并列不占位）
来源：http://xjf.ivvv.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qiz.zdbjq.cn

[Q57] 行号
来源：http://meo.gotoacloud.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bxd.c1oappe.top

[Q58] 累计求和
来源：http://hfy.chenzaomai.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fwd.wangshuangyany.cn

[Q59] 分组内累计
来源：http://cha.cashguo.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ebn.tian-w.cn

[Q60] 取上一行 / 下一行
来源：http://tfw.iojbl.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kxj.hesvh.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ibf.dianchejie.cn

[Q61] 移动平均
来源：http://ahk.gotoacloud.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://imc.ctjpmb.com

[Q62] 分组占比
来源：http://kum.jinyuanbaomall.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://plx.hammf.cn

[Q63] 开启事务
来源：http://ivm.zycfv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dfo.daxiang520.top

[Q64] 提交事务
来源：http://ylk.zdbjq.cn

COMMIT;
来源：http://har.nanxinkj.top

[Q65] 回滚事务
来源：http://etm.iojbl.cn

ROLLBACK;
来源：http://gbp.fanxiaobao.xyz

[Q66] 行锁查询
来源：http://ebk.jqgfzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ugx.dianchejie.cn

[Q67] 设置隔离级别
来源：http://hqg.nanxuanxn.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://edu.fzhhl.top

[Q68] 保存点
来源：http://gkh.shanyushiyangkeji.top

SAVEPOINT sp1;
来源：http://zrs.hammf.cn

ROLLBACK TO sp1;
来源：http://awe.jinghuilouyu.cn

[Q69] 查看执行计划
来源：http://yhf.xziqi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lrc.mhx1999.top

[Q70] 更新统计信息
来源：http://rek.sjlbkw.cn

ANALYZE TABLE users;
来源：http://gol.jianghu66.top

[Q71] 查看建表语句
来源：http://ftm.svipenyu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yun.zhijiandao.cn

[Q72] 查看索引
来源：http://lbc.sweek.top

SHOW INDEX FROM users;
来源：http://yxm.zhongyouzk.top

[Q73] 查看表状态
来源：http://ugp.fanxiaobao.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://qwe.c1oappe.top

[Q74] 强制使用索引
来源：http://lro.xinyue.icu

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mnb.guannengcc.top

[Q75] 日期格式化
来源：http://syp.dianchejie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vpl.smart0.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://odj.yuanzhike.top

[Q76] 按天统计
来源：http://amp.cqqwz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zwh.havefunace.top

[Q77] 时间加减
来源：http://zgf.nanxuanxn.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dvm.yangfankeji.com

[Q78] 当前时间
来源：http://qib.shanyushiyangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kpr.xylfe.cn

[Q79] 字符串拼接
来源：http://vhz.yuxming.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yuv.jqgufenzy.top

[Q80] 字符串截取
来源：http://quv.hcnkem.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://eor.zhiwuduotai.top

[Q81] 字符串替换
来源：http://ngr.wangshuangyany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fge.zhaomingkeji.xyz

[Q82] 字符长度与字节长度
来源：http://var.cucudq.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://avw.jyoumei.cn

[Q83] 大小写转换
来源：http://ynr.bjfxy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pmy.ydjk.org.cn

[Q84] 去除首尾空格
来源：http://ncq.nwbrower.top

SELECT TRIM(name) FROM users;
来源：http://cgv.yj20258.top

[Q85] 数值取整
来源：http://xbg.quarkkingdee.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sfx.xylfe.cn

[Q86] 读取 JSON 字段
来源：http://uwc.nanxuanxn.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://paj.cdnleiting.top

[Q87] JSON 字段做条件
来源：http://vqt.shanyushiyangtech.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xki.guannengcc.top

[Q88] 行转列（条件聚合）
来源：http://gil.vehdjk.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lxg.aibaodan.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hcv.yuxming.cn

[Q89] 判断表是否存在
来源：http://qyf.nwbrower.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ftf.cucudq.cn

[Q90] 生成序号列
来源：http://exs.vehdjk.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://maw.52xcode.cn

================================================================================
来源：http://xod.quarkkingdee.top

R. Bash 专题
来源：http://tos.redwolf501.top

================================================================================
来源：http://thr.aizwys.cn

[R01] shebang 与严格模式
来源：http://cwj.kuanghao11.cn

#!/usr/bin/env bash
来源：http://hst.shanyushiyangkeji.top

set -euo pipefail
来源：http://upy.tanke756.top

[R02] 变量赋值与使用
来源：http://yuh.cucudq.cn

name="Tom"; echo "$name"
来源：http://glh.ctjpmb.com

[R03] 只读变量
来源：http://nwf.zhengqikj.top

readonly PI=3.14
来源：http://rme.sysykeji.top

[R04] 位置参数
来源：http://imw.wangshuangyany.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xlt.yanxiufei.cn

[R05] 参数默认值
来源：http://xpw.svipenyu.cn

name="${1:-default}"
来源：http://gky.jianghu66.top

[R06] 判断命令是否存在
来源：http://grd.tanke756.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hqz.yuanzhike.top

[R07] if 判断文件
来源：http://mou.jinghuilouyu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hoj.nanxuanxn.top

[R08] 数值比较
来源：http://niv.kuanghao11.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://doj.guannengcc.top

[R09] 字符串比较
来源：http://qvu.aizwys.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pfd.yfazqb.com

[R10] 正则匹配
来源：http://irh.yvedp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://itd.fzhhl.top

[R11] case 多分支
来源：http://hrh.zhengqikj.top

case "$1" in
来源：http://chg.chenlongwang.top

start) echo "启动" ;;
来源：http://twx.xuanzx.com

stop)  echo "停止" ;;
来源：http://anh.tarul.cn

*)     echo "未知命令" ;;
来源：http://lmy.fktsv.cn

esac
来源：http://owq.zhixingplan.top

[R12] for 遍历文件
来源：http://tqa.hcnkem.com

for f in *.txt; do echo "$f"; done
来源：http://evb.jqgufenzy.top

[R13] for 计数循环
来源：http://yyx.nanxuanxn.top

for i in {1..10}; do echo "$i"; done
来源：http://nti.aizwys.cn

[R14] C 风格 for
来源：http://ksk.zhongyouzk.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sxc.vqdsnc.cn

[R15] while 逐行读文件
来源：http://qlk.ctjpmb.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fzf.gogol.net.cn

[R16] until 等待条件
来源：http://zfk.xziqi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://enf.dashuyun.cn

[R17] 数组定义与取值
来源：http://bhc.epnwcf.com

arr=(a b c); echo "${arr[0]}"
来源：http://vwp.yueranfly.top

[R18] 遍历数组
来源：http://dqb.xinyue.icu

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hzq.aibaodan.cn

[R19] 数组长度
来源：http://vlj.wangdashe.top

echo "${#arr[@]}"
来源：http://tbg.cqqwz.cn

[R20] 关联数组（字典）
来源：http://yqd.xingfuxueyuan.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vol.yueranfly.top

[R21] 字符串长度
来源：http://mqm.zhongyouzk.top

echo "${#s}"
来源：http://rcl.epnwcf.com

[R22] 截取子串
来源：http://zfi.cucudq.cn

echo "${s:0:5}"
来源：http://grk.jianghu66.top

[R23] 字符串替换
来源：http://qou.ehwqpu.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://htg.sysykeji.top

[R24] 大小写转换
来源：http://skd.sxryk.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sak.daxiang520.top

[R25] 去后缀 / 去前缀
来源：http://mtj.zhiwuduotai.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://yhi.kuanghao11.cn

[R26] 命令替换
来源：http://zox.jinqigfzy.top

now=$(date +%F); echo "$now"
来源：http://uaw.ywan-chungtsiang.top

[R27] 算术展开
来源：http://uev.shuidangran.top

echo $((1 + 2 * 3))
来源：http://kir.zdqjudy.top

[R28] 浮点运算
来源：http://mkr.havefunace.top

echo "scale=2; 10/3" | bc
来源：http://kgb.chenzaomai.com

[R29] 定义函数
来源：http://zux.9152youxi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ijf.chenzaomai.com

[R30] 函数返回状态码
来源：http://eem.gogol.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://gsn.jiagoushi.top

[R31] 局部变量
来源：http://tpv.aibaodan.cn

f() { local x=1; echo "$x"; }
来源：http://nfs.jyoumei.cn

[R32] 参数个数校验
来源：http://ojo.dianchejie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jwe.cheryme.top

[R33] 捕获错误并提示行号
来源：http://bji.zhijiandao.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uex.vehdjk.com

[R34] 退出时清理
来源：http://dfs.pengpengdd.cyou

trap 'rm -f "$tmp"' EXIT
来源：http://umv.yj20258.top

[R35] 后台执行并等待
来源：http://vex.cqqwz.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://eny.gotoacloud.top

[R36] 并发执行多个任务
来源：http://bjv.xinyue.icu

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wwp.yanxiufei.cn

[R37] 把输出赋给变量
来源：http://xjc.jiagoushi.top

files=$(ls -1)
来源：http://kka.daria6918.cn

[R38] 管道串联
来源：http://jci.jinqigfzy.top

cat a.txt | grep -i error | wc -l
来源：http://lln.yuanzhike.top

[R39] 重定向标准输出与错误
来源：http://zxg.bbcook.cn

cmd > out.log 2>&1
来源：http://pff.tanke756.top

[R40] 追加写日志
来源：http://wlz.epnwcf.com

echo "log" >> out.log
来源：http://vgz.hywenlv.cn

[R41] 丢弃输出
来源：http://msf.hysaishi.cn

cmd >/dev/null 2>&1
来源：http://bmw.fehbvm.com

[R42] 输入重定向
来源：http://glg.ybcxt.top

wc -l < a.txt
来源：http://ehs.aizwys.cn

[R43] 按名字查找文件
来源：http://lmu.yuxming.cn

find . -name "*.log" -type f
来源：http://fuz.chenzaomai.com

[R44] 按修改时间查找
来源：http://ylt.cucudq.cn

find . -mtime -7 -type f
来源：http://czw.jqgfzy.top

[R45] 批量删除
来源：http://zwx.fengsongda.top

find . -name "*.tmp" -delete
来源：http://fco.zhengqikj.top

[R46] 递归替换文件内容
来源：http://dka.ppjwa.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zuf.pycfn.com

[R47] sed 单行替换
来源：http://zck.jiagoushi.top

sed -i 's/foo/bar/g' a.txt
来源：http://oxz.zhengqikj.top

[R48] awk 取指定列
来源：http://mmm.52xcode.cn

awk '{print $1, $3}' a.txt
来源：http://rrw.chenjidiqi.icu

[R49] awk 带条件
来源：http://kuh.yueranfly.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ouz.hnxiangtu.top

[R50] awk 求和
来源：http://vay.ydzc1.top

awk '{s += $2} END {print s}' a.txt
来源：http://nht.zhoulong.xyz

[R51] 排序去重取前几
来源：http://cmf.hesvh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://avi.cqqwz.cn

[R52] 统计行数
来源：http://lqg.fehbvm.com

wc -l a.txt
来源：http://jwf.zhiwuduotai.top

[R53] 查看文件头与实时尾
来源：http://ffm.hfpthk.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fzj.yonumen.top

[R54] 比较两个文件
来源：http://qgz.guannengcc.top

diff a.txt b.txt
来源：http://dom.jqgufenzy.top

[R55] 压缩与解压
来源：http://cbe.yuxming.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gvm.hnxiangtu.top

[R56] 远程拷贝
来源：http://dxk.hnxiangtu.top

scp file user@host:/path/
来源：http://vgp.yonumen.top

[R57] 远程执行命令
来源：http://ssf.ybcxt.top

ssh user@host 'uptime'
来源：http://ikq.zhoulong.xyz

[R58] 下载文件
来源：http://wgs.hnqzz.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lkg.nanxinkj.top

[R59] 发 POST JSON
来源：http://mpq.pycfn.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kzf.yongpay.top

[R60] 只看 HTTP 状态码
来源：http://bod.cqqwz.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yub.jlsjyb.cn

[R61] 磁盘占用
来源：http://uct.shanyushiyangkeji.top

df -h;  du -sh *
来源：http://ltw.cashguo.top

[R62] 找最占空间的文件
来源：http://uin.iojbl.cn

du -ah . | sort -rh | head -10
来源：http://hcw.zhongyouzk.top

[R63] 内存与进程
来源：http://stl.mhx1999.top

free -h;  ps aux | grep nginx
来源：http://ock.aizwys.cn

[R64] 结束进程
来源：http://qbc.cheryme.top

kill -9 $(pgrep -f app.py)
来源：http://mst.xuanzx.com

[R65] 查看端口占用
来源：http://gtl.zycfv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qlb.yanxiufei.cn

[R66] 定时任务
来源：http://jao.iojbl.cn

crontab -e;  crontab -l
来源：http://ivv.hnxiangtu.top

[R67] 生成随机十六进制串
来源：http://vas.shuidangran.top

openssl rand -hex 16
来源：http://fwx.dashuyun.cn

[R68] 计算文件校验值
来源：http://lkp.sjlbkw.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lmc.zhiwuduotai.top

[R69] 生成随机密码
来源：http://bvh.ydzc1.top


<!-- 参考信息 -->