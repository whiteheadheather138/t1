代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tgh.zdqjudy.top

[Q18] 模糊匹配
来源：http://vnm.xuetiantiany.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://brf.xuanzx.com

[Q19] 范围查询
来源：http://agv.yvedp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://itz.yfazqb.com

[Q20] IN 列表
来源：http://foe.xuanzx.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rrw.iojbl.cn

[Q21] 空值判断
来源：http://dyd.jinyuanbaomall.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fzv.yongpay.top

[Q22] 排序
来源：http://oon.shanyushiyangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jon.yangfankeji.com

[Q23] 分页
来源：http://tap.dashuyun.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://err.xziqi.cn

[Q24] 去重
来源：http://cbb.wangdashe.top

SELECT DISTINCT city FROM users;
来源：http://sua.guowangkeji.top

[Q25] 只取前 N 条
来源：http://mvv.jqgufenzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fxw.xuanzx.com

[Q26] 计数
来源：http://jrf.yueranfly.top

SELECT COUNT(*) FROM users;
来源：http://qci.vehdjk.com

[Q27] 条件计数
来源：http://ecz.hfpthk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hre.xylfe.cn

[Q28] 求和与平均
来源：http://ilv.fktsv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://clv.redwolf501.top

[Q29] 最大最小值
来源：http://mth.yangfankeji.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://did.feifeiyinyue.top

[Q30] 分组统计
来源：http://igc.hesvh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mdx.andypj.xyz

[Q31] 分组后过滤
来源：http://uli.yongpay.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tcr.yongpay.top

[Q32] 分组拼接字符串
来源：http://dry.ctjpmb.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fjd.bbcook.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://elz.c1oappe.top

[Q33] 多列分组
来源：http://zdl.xuetiantiany.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vsk.ydjk.org.cn

[Q34] 每组取第一条
来源：http://rtu.sufxvd.cn

SELECT * FROM (
来源：http://aru.jqgufenzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nfg.yongpay.top

) t WHERE rn = 1;
来源：http://euh.mhx1999.top

[Q35] 内连接
来源：http://ctz.andypj.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tpt.xinyue.icu

[Q36] 左连接
来源：http://pli.316326.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ogj.ppjwa.cn

[Q37] 右连接
来源：http://jhf.shanyushiyangkeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://acc.xingfuxueyuan.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://dmf.jyoumei.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lrl.shuidangran.top

[Q39] 自连接（查上下级）
来源：http://mim.yueranfly.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://uqm.hcnkem.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wlp.cucudq.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xdm.shuidangran.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pwc.nanxinkj.top

[Q41] 多表连接
来源：http://upg.vqdsnc.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wbc.yueranfly.top

JOIN users u ON u.id = o.user_id
来源：http://lnl.fktsv.cn

JOIN products p ON p.id = o.product_id;
来源：http://haa.yanxiufei.cn

[Q42] 连接条件附加过滤
来源：http://gfr.xylfe.cn

SELECT u.name, o.amount FROM users u
来源：http://iik.xingfuxueyuan.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dbe.cdnleiting.top

[Q43] 标量子查询
来源：http://rpd.havefunace.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hfy.gzhubu.top

[Q44] IN 子查询
来源：http://uli.0kj1m.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zim.jlsjyb.cn

[Q45] EXISTS 判断存在
来源：http://ilp.jinyuanbaomall.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mbt.316326.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://fvd.andypj.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kds.fanxiaobao.xyz

[Q47] 与平均值比较
来源：http://drr.dianchejie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zjz.aizwys.cn

[Q48] CTE 公用表表达式
来源：http://efe.ctjpmb.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ysx.sysykeji.top

SELECT * FROM t WHERE c > 5;
来源：http://buk.andypj.xyz

[Q49] 更新单行
来源：http://wwr.yj202588.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dxm.ydjk.org.cn

[Q50] 批量更新
来源：http://cmk.bbcook.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xmt.c1oappe.top

[Q51] 用子查询更新
来源：http://fpr.zhijiandao.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wjk.zhijiandao.cn

[Q52] 删除指定行
来源：http://hha.yvedp.cn

DELETE FROM users WHERE id = 10;
来源：http://beg.guowangkeji.top

[Q53] 按条件删除
来源：http://ywf.shangyingyoupin.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ipr.yonumen.top

[Q54] 清空表
来源：http://gpb.yuanzhike.top

TRUNCATE TABLE logs;
来源：http://wqn.sxryk.cn

[Q55] 排名（并列占位）
来源：http://ryo.kuanghao11.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kcf.hongshengwenyu.top

[Q56] 密集排名（并列不占位）
来源：http://ldt.jianghu66.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://avu.yuanzhike.top

[Q57] 行号
来源：http://ogg.zhixingplan.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fkx.ydjk.org.cn

[Q58] 累计求和
来源：http://bcl.ehwqpu.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://okd.birdmap.top

[Q59] 分组内累计
来源：http://azo.shuidangran.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://igs.yj202588.top

[Q60] 取上一行 / 下一行
来源：http://qes.shanyushiyangkeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rbm.tarul.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xhx.gzhubu.top

[Q61] 移动平均
来源：http://zli.chenjidiqi.icu

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lem.zhaomingkeji.xyz

[Q62] 分组占比
来源：http://riu.epnwcf.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dwk.ydzc1.top

[Q63] 开启事务
来源：http://ndq.yvedp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://htk.shanyushiyangtech.top

[Q64] 提交事务
来源：http://pwc.jianghu66.top

COMMIT;
来源：http://uem.jqgfzy.top

[Q65] 回滚事务
来源：http://gbd.ctjpmb.com

ROLLBACK;
来源：http://qcg.epnwcf.com

[Q66] 行锁查询
来源：http://ipz.cucudq.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://otb.tarul.cn

[Q67] 设置隔离级别
来源：http://alf.zhixingplan.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dqy.shuidangran.top

[Q68] 保存点
来源：http://eit.xinyue.icu

SAVEPOINT sp1;
来源：http://mgt.fanxiaobao.xyz

ROLLBACK TO sp1;
来源：http://wsc.9152youxi.cn

[Q69] 查看执行计划
来源：http://hoz.cucudq.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bjx.zhaomingkeji.xyz

[Q70] 更新统计信息
来源：http://dbj.zdbjq.cn

ANALYZE TABLE users;
来源：http://deu.guannengcc.top

[Q71] 查看建表语句
来源：http://fbt.guowangkeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jnl.hcnkem.com

[Q72] 查看索引
来源：http://omd.andypj.xyz

SHOW INDEX FROM users;
来源：http://xml.sweek.top

[Q73] 查看表状态
来源：http://xxf.shuidangran.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vto.fehbvm.com

[Q74] 强制使用索引
来源：http://jfu.ppjwa.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dul.yfazqb.com

[Q75] 日期格式化
来源：http://hjz.ybcxt.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rjg.zhongyouzk.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qyj.shzxlz.cn

[Q76] 按天统计
来源：http://cbt.yanxiufei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fnf.ywan-chungtsiang.top

[Q77] 时间加减
来源：http://ywa.ehwqpu.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ehq.xuanzx.com

[Q78] 当前时间
来源：http://vsg.gogol.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fgo.zhengqikj.top

[Q79] 字符串拼接
来源：http://rdq.tianlin.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mnc.mhx1999.top

[Q80] 字符串截取
来源：http://bil.jqgufenzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xlo.vqdsnc.cn

[Q81] 字符串替换
来源：http://mtu.cucudq.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qos.cucudq.cn

[Q82] 字符长度与字节长度
来源：http://pdd.mhx1999.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oai.daxiang520.top

[Q83] 大小写转换
来源：http://jyy.bjfxy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pcp.fehbvm.com

[Q84] 去除首尾空格
来源：http://yoy.dashuyun.cn

SELECT TRIM(name) FROM users;
来源：http://hzc.iojbl.cn

[Q85] 数值取整
来源：http://lsy.sjlbkw.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://scu.havefunace.top

[Q86] 读取 JSON 字段
来源：http://bvq.ehwqpu.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hwq.xylfe.cn

[Q87] JSON 字段做条件
来源：http://cig.hysaishi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jda.svipenyu.cn

[Q88] 行转列（条件聚合）
来源：http://rqw.fengsongda.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ync.ydjk.org.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hex.hfpthk.cn

[Q89] 判断表是否存在
来源：http://clw.gaohongyu789.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ote.ivvv.top

[Q90] 生成序号列
来源：http://xsj.vqdsnc.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ylw.smart0.xyz

================================================================================
来源：http://ixi.sweek.top

R. Bash 专题
来源：http://bai.dianchejie.cn

================================================================================
来源：http://grs.aizwys.cn

[R01] shebang 与严格模式
来源：http://xrj.zdqjudy.top

#!/usr/bin/env bash
来源：http://lie.zhoulong.xyz

set -euo pipefail
来源：http://cfy.pycfn.com

[R02] 变量赋值与使用
来源：http://kks.fehbvm.com

name="Tom"; echo "$name"
来源：http://fxn.chenlongwang.top

[R03] 只读变量
来源：http://csa.sufxvd.cn

readonly PI=3.14
来源：http://vft.dianchejie.cn

[R04] 位置参数
来源：http://cnp.zhengqikj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ltk.guannengcc.top

[R05] 参数默认值
来源：http://enz.andypj.xyz

name="${1:-default}"
来源：http://qoe.chenzaomai.com

[R06] 判断命令是否存在
来源：http://gwy.xziqi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tpt.birdmap.top

[R07] if 判断文件
来源：http://cnt.wangdashe.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jvr.snrcjt.cn

[R08] 数值比较
来源：http://ofs.hammf.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zrs.mhx1999.top

[R09] 字符串比较
来源：http://lwz.ydjk.org.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kkh.fzhhl.top

[R10] 正则匹配
来源：http://xnl.yanxiufei.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://com.sxryk.cn

[R11] case 多分支
来源：http://xno.meibo888.top

case "$1" in
来源：http://nfd.xylfe.cn

start) echo "启动" ;;
来源：http://mda.shuidangran.top

stop)  echo "停止" ;;
来源：http://hdc.ehwqpu.com

*)     echo "未知命令" ;;
来源：http://trh.chenzaomai.com

esac
来源：http://wxo.dianchejie.cn

[R12] for 遍历文件
来源：http://nxb.zhoulong.xyz

for f in *.txt; do echo "$f"; done
来源：http://ywn.hcnkem.com

[R13] for 计数循环
来源：http://fhj.fehbvm.com

for i in {1..10}; do echo "$i"; done
来源：http://owk.xziqi.cn

[R14] C 风格 for
来源：http://wxu.aizwys.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rcr.yj20258.top

[R15] while 逐行读文件
来源：http://ezo.shanyushiyangkeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gpd.fengsongda.top

[R16] until 等待条件
来源：http://twc.yfazqb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lss.snrcjt.cn

[R17] 数组定义与取值
来源：http://mav.iojbl.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ywq.redwolf501.top

[R18] 遍历数组
来源：http://jqi.hnxiangtu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gvx.hnxiangtu.top

[R19] 数组长度
来源：http://yue.cqqwz.cn

echo "${#arr[@]}"
来源：http://zck.sysykeji.top

[R20] 关联数组（字典）
来源：http://ror.yangfankeji.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cvj.aizwys.cn

[R21] 字符串长度
来源：http://jki.quarkkingdee.top

echo "${#s}"
来源：http://joa.ivvv.top

[R22] 截取子串
来源：http://mtc.xinyue.icu

echo "${s:0:5}"
来源：http://qri.jinqigfzy.top

[R23] 字符串替换
来源：http://wsh.fktsv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://knt.svipenyu.cn

[R24] 大小写转换
来源：http://mjn.svipenyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://dbq.jqgufenzy.top

[R25] 去后缀 / 去前缀
来源：http://efq.316326.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://hnn.jinyuanbaomall.cn

[R26] 命令替换
来源：http://ozb.c1oappe.top

now=$(date +%F); echo "$now"
来源：http://amf.haohaochexian.top

[R27] 算术展开
来源：http://vxb.fktsv.cn

echo $((1 + 2 * 3))
来源：http://jqp.zycfv.cn

[R28] 浮点运算
来源：http://xcp.xuetiantiany.cn

echo "scale=2; 10/3" | bc
来源：http://puy.jqgufenzy.top

[R29] 定义函数
来源：http://wzz.fzhhl.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ymo.sysykeji.top

[R30] 函数返回状态码
来源：http://oii.yangfankeji.com

f() { return 0; }; f || echo "失败了"
来源：http://coe.c1oappe.top

[R31] 局部变量
来源：http://zrc.tian-w.cn

f() { local x=1; echo "$x"; }
来源：http://ehj.0kj1m.cn

[R32] 参数个数校验
来源：http://kkh.jlsjyb.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kwv.nanxinkj.top

[R33] 捕获错误并提示行号
来源：http://huv.chenjidiqi.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ntr.shanyushiyangkeji.top

[R34] 退出时清理
来源：http://zyd.zdqjudy.top

trap 'rm -f "$tmp"' EXIT
来源：http://lvh.hywenlv.cn

[R35] 后台执行并等待
来源：http://cdb.zhijiandao.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://owj.fanxiaobao.xyz

[R36] 并发执行多个任务
来源：http://rir.daria6918.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ckp.cdnleiting.top

[R37] 把输出赋给变量
来源：http://wtj.uphjek.com

files=$(ls -1)
来源：http://egi.hesvh.cn

[R38] 管道串联
来源：http://vps.chenlongwang.top

cat a.txt | grep -i error | wc -l
来源：http://cdc.vqdsnc.cn

[R39] 重定向标准输出与错误
来源：http://hpp.gotoacloud.top

cmd > out.log 2>&1
来源：http://nby.tanke756.top

[R40] 追加写日志
来源：http://wjy.mhx1999.top

echo "log" >> out.log
来源：http://ziy.vehdjk.com

[R41] 丢弃输出
来源：http://lax.gaohongyu789.top

cmd >/dev/null 2>&1
来源：http://fkf.xziqi.cn

[R42] 输入重定向
来源：http://igl.shuidangran.top

wc -l < a.txt
来源：http://dwt.gzhubu.top

[R43] 按名字查找文件
来源：http://oce.cashguo.top

find . -name "*.log" -type f
来源：http://gmb.sufxvd.cn

[R44] 按修改时间查找
来源：http://hct.hywenlv.cn

find . -mtime -7 -type f
来源：http://oug.yuxming.cn

[R45] 批量删除
来源：http://ylo.dashuyun.cn

find . -name "*.tmp" -delete
来源：http://voj.tianlin.xyz

[R46] 递归替换文件内容
来源：http://cns.52xcode.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qev.iojbl.cn

[R47] sed 单行替换
来源：http://xch.shanyushiyangtech.top

sed -i 's/foo/bar/g' a.txt
来源：http://bpm.svipenyu.cn

[R48] awk 取指定列
来源：http://jjv.yj20258888.top

awk '{print $1, $3}' a.txt
来源：http://tkc.sweek.top

[R49] awk 带条件
来源：http://sph.hcnkem.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blc.hcnkem.com

[R50] awk 求和
来源：http://qtb.bbcook.cn

awk '{s += $2} END {print s}' a.txt
来源：http://unx.hywenlv.cn

[R51] 排序去重取前几
来源：http://spk.52xcode.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sof.bjfxy.top

[R52] 统计行数
来源：http://dwi.cashguo.top

wc -l a.txt
来源：http://eff.quarkkingdee.top

[R53] 查看文件头与实时尾
来源：http://rrw.tian-w.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xef.shuidangran.top

[R54] 比较两个文件
来源：http://ija.wangdashe.top

diff a.txt b.txt
来源：http://akb.52xcode.cn

[R55] 压缩与解压
来源：http://kqq.yj20258888.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://byh.yueranfly.top

[R56] 远程拷贝
来源：http://xlx.vehdjk.com

scp file user@host:/path/
来源：http://sll.hysaishi.cn

[R57] 远程执行命令
来源：http://ana.zhongyouzk.top

ssh user@host 'uptime'
来源：http://axe.aizwys.cn

[R58] 下载文件
来源：http://aeu.zdqjudy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://esk.xylfe.cn

[R59] 发 POST JSON
来源：http://odv.wangshuangyany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://afn.gogol.net.cn

[R60] 只看 HTTP 状态码
来源：http://pnj.yongpay.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rbf.snrcjt.cn

[R61] 磁盘占用
来源：http://uds.sufxvd.cn

df -h;  du -sh *
来源：http://hak.shanyushiyangkeji.top

[R62] 找最占空间的文件
来源：http://voz.sysykeji.top

du -ah . | sort -rh | head -10
来源：http://cth.fehbvm.com

[R63] 内存与进程
来源：http://znz.vehdjk.com

free -h;  ps aux | grep nginx
来源：http://vmd.andypj.xyz

[R64] 结束进程
来源：http://zwr.shanyushiyangkeji.top

kill -9 $(pgrep -f app.py)
来源：http://tie.yueranfly.top

[R65] 查看端口占用
来源：http://wsb.9152youxi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cva.quarkkingdee.top

[R66] 定时任务
来源：http://sxw.yanxiufei.cn

crontab -e;  crontab -l
来源：http://ovz.hfpthk.cn

[R67] 生成随机十六进制串
来源：http://hhn.shanyushiyangkeji.top


<!-- 参考信息 -->