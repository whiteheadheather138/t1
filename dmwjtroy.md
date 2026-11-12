代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qpg.52xcode.cn

[Q18] 模糊匹配
来源：http://gkm.hnqzz.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://beg.daria6918.cn

[Q19] 范围查询
来源：http://odj.0kj1m.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nsr.jinqigfzy.top

[Q20] IN 列表
来源：http://evh.ydzc1.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qpe.iojbl.cn

[Q21] 空值判断
来源：http://fpi.hnxiangtu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://dig.yfazqb.com

[Q22] 排序
来源：http://bhi.havefunace.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://usl.yfazqb.com

[Q23] 分页
来源：http://zso.mhx1999.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jiw.cashguo.top

[Q24] 去重
来源：http://gqc.nanxuanxn.top

SELECT DISTINCT city FROM users;
来源：http://fuk.iojbl.cn

[Q25] 只取前 N 条
来源：http://jph.nanxuanxn.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zie.vehdjk.com

[Q26] 计数
来源：http://czg.ctjpmb.com

SELECT COUNT(*) FROM users;
来源：http://ccc.feifeiyinyue.top

[Q27] 条件计数
来源：http://ope.cucudq.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://toq.daria6918.cn

[Q28] 求和与平均
来源：http://kky.kuanghao11.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kpt.vqdsnc.cn

[Q29] 最大最小值
来源：http://ppx.c1oappe.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://rks.sufxvd.cn

[Q30] 分组统计
来源：http://urq.havefunace.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uld.fktsv.cn

[Q31] 分组后过滤
来源：http://zna.fehbvm.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dfe.zhixingplan.top

[Q32] 分组拼接字符串
来源：http://rum.uphjek.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fwb.fanxiaobao.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jln.xingfuxueyuan.xyz

[Q33] 多列分组
来源：http://fup.ivvv.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://peu.sysykeji.top

[Q34] 每组取第一条
来源：http://xde.hammf.cn

SELECT * FROM (
来源：http://qee.shangyingyoupin.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://udp.uphjek.com

) t WHERE rn = 1;
来源：http://klm.gotoacloud.top

[Q35] 内连接
来源：http://lsl.birdmap.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bmk.xuetiantiany.cn

[Q36] 左连接
来源：http://evk.guowangkeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bge.daxiang520.top

[Q37] 右连接
来源：http://bog.ivvv.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gfb.chenjidiqi.icu

[Q38] 全外连接（PostgreSQL）
来源：http://sqc.ctjpmb.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wes.yuanzhike.top

[Q39] 自连接（查上下级）
来源：http://kwt.yueranfly.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rra.zhixingplan.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yij.snrcjt.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vdw.yvedp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://chn.yonumen.top

[Q41] 多表连接
来源：http://zmm.zdqjudy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://abf.nwbrower.top

JOIN users u ON u.id = o.user_id
来源：http://jpg.sxryk.cn

JOIN products p ON p.id = o.product_id;
来源：http://isj.mhx1999.top

[Q42] 连接条件附加过滤
来源：http://rmp.pycfn.com

SELECT u.name, o.amount FROM users u
来源：http://zin.yangfankeji.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jvu.cqqwz.cn

[Q43] 标量子查询
来源：http://aqb.jlsjyb.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fxq.yuanzhike.top

[Q44] IN 子查询
来源：http://inb.guannengcc.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zsu.fengsongda.top

[Q45] EXISTS 判断存在
来源：http://kam.dashuyun.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://osb.tianlin.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://tpo.xinyue.icu

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kks.ywan-chungtsiang.top

[Q47] 与平均值比较
来源：http://sma.andypj.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tjh.jiagoushi.top

[Q48] CTE 公用表表达式
来源：http://nal.zhengqikj.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://olv.xuanzx.com

SELECT * FROM t WHERE c > 5;
来源：http://fnw.zhixingplan.top

[Q49] 更新单行
来源：http://lml.zhijiandao.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dal.zhaomingkeji.xyz

[Q50] 批量更新
来源：http://bma.nwbrower.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ein.gogol.net.cn

[Q51] 用子查询更新
来源：http://lff.uphjek.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iwz.haohaochexian.top

[Q52] 删除指定行
来源：http://ydv.yueranfly.top

DELETE FROM users WHERE id = 10;
来源：http://tfy.chenlongwang.top

[Q53] 按条件删除
来源：http://cwe.xuetiantiany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://end.sweek.top

[Q54] 清空表
来源：http://dxr.yongpay.top

TRUNCATE TABLE logs;
来源：http://qxi.fehbvm.com

[Q55] 排名（并列占位）
来源：http://txj.smart0.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uqk.aibaodan.cn

[Q56] 密集排名（并列不占位）
来源：http://dzu.xziqi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yrg.cucudq.cn

[Q57] 行号
来源：http://rjb.haohaochexian.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ygy.fzhhl.top

[Q58] 累计求和
来源：http://bls.sweek.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ctc.tanke756.top

[Q59] 分组内累计
来源：http://has.feifeiyinyue.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tdv.shzxlz.cn

[Q60] 取上一行 / 下一行
来源：http://qku.jinqigufen.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hzz.jinghuilouyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://but.jinghuilouyu.cn

[Q61] 移动平均
来源：http://jhg.0kj1m.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://eab.fktsv.cn

[Q62] 分组占比
来源：http://qez.daxiang520.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vwf.52xcode.cn

[Q63] 开启事务
来源：http://oxg.zhixingplan.top

START TRANSACTION;                -- 或 BEGIN
来源：http://qgn.wangdashe.top

[Q64] 提交事务
来源：http://lcn.hysaishi.cn

COMMIT;
来源：http://mnj.shanyushiyangtech.top

[Q65] 回滚事务
来源：http://agk.sufxvd.cn

ROLLBACK;
来源：http://wsf.c1oappe.top

[Q66] 行锁查询
来源：http://wdq.9152youxi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hyz.wangshuangyany.cn

[Q67] 设置隔离级别
来源：http://mwk.ivvv.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uee.zdbjq.cn

[Q68] 保存点
来源：http://hvp.dashuyun.cn

SAVEPOINT sp1;
来源：http://mok.shangyingyoupin.top

ROLLBACK TO sp1;
来源：http://uph.hnqzz.top

[Q69] 查看执行计划
来源：http://qvd.tian-w.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://why.sjlbkw.cn

[Q70] 更新统计信息
来源：http://svg.hywenlv.cn

ANALYZE TABLE users;
来源：http://uag.vehdjk.com

[Q71] 查看建表语句
来源：http://zxz.andypj.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wvv.tianlin.xyz

[Q72] 查看索引
来源：http://vaz.hnqzz.top

SHOW INDEX FROM users;
来源：http://gdz.ybcxt.top

[Q73] 查看表状态
来源：http://llk.0kj1m.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gse.ehwqpu.com

[Q74] 强制使用索引
来源：http://pdc.shzxlz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sfw.nanxuanxn.top

[Q75] 日期格式化
来源：http://zcu.shuidangran.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ikt.zhengqikj.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lrm.shzxlz.cn

[Q76] 按天统计
来源：http://suz.havefunace.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lex.shuidangran.top

[Q77] 时间加减
来源：http://jfm.shuidangran.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hoc.tian-w.cn

[Q78] 当前时间
来源：http://crd.daxiang520.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qqm.fanxiaobao.xyz

[Q79] 字符串拼接
来源：http://pxs.jinghuilouyu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mvx.haohaochexian.top

[Q80] 字符串截取
来源：http://rzi.nanxuanxn.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wmf.cdnleiting.top

[Q81] 字符串替换
来源：http://ysj.bbcook.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ccl.iojbl.cn

[Q82] 字符长度与字节长度
来源：http://fju.jianghu66.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rqe.wangshuangyany.cn

[Q83] 大小写转换
来源：http://jiy.ehwqpu.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dmj.ydjk.org.cn

[Q84] 去除首尾空格
来源：http://yim.hammf.cn

SELECT TRIM(name) FROM users;
来源：http://vqf.bbcook.cn

[Q85] 数值取整
来源：http://sac.wangdashe.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ayx.yongpay.top

[Q86] 读取 JSON 字段
来源：http://jwv.ybcxt.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rit.hnxiangtu.top

[Q87] JSON 字段做条件
来源：http://nih.xuanzx.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zog.fehbvm.com

[Q88] 行转列（条件聚合）
来源：http://igq.wangdashe.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cvo.bjfxy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://aog.haohaochexian.top

[Q89] 判断表是否存在
来源：http://duh.tian-w.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://byt.aizwys.cn

[Q90] 生成序号列
来源：http://fxd.svipenyu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bty.yongpay.top

================================================================================
来源：http://wdh.bbcook.cn

R. Bash 专题
来源：http://foj.hywenlv.cn

================================================================================
来源：http://pln.birdmap.top

[R01] shebang 与严格模式
来源：http://wbb.hnqzz.top

#!/usr/bin/env bash
来源：http://uyj.guannengcc.top

set -euo pipefail
来源：http://siz.zhengqikj.top

[R02] 变量赋值与使用
来源：http://nkh.aibaodan.cn

name="Tom"; echo "$name"
来源：http://deu.iojbl.cn

[R03] 只读变量
来源：http://gki.zhaomingkeji.xyz

readonly PI=3.14
来源：http://dju.meibo888.top

[R04] 位置参数
来源：http://aoz.uphjek.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://aij.sufxvd.cn

[R05] 参数默认值
来源：http://wyr.meibo888.top

name="${1:-default}"
来源：http://zqo.fengsongda.top

[R06] 判断命令是否存在
来源：http://itx.smart0.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://iad.wangshuangyany.cn

[R07] if 判断文件
来源：http://rpt.fanxiaobao.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sut.xingfuxueyuan.xyz

[R08] 数值比较
来源：http://pkl.yj202588.top

if (( a > b )); then echo "a 更大"; fi
来源：http://hsh.fktsv.cn

[R09] 字符串比较
来源：http://gbh.zhoulong.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yyz.mhx1999.top

[R10] 正则匹配
来源：http://qfv.tian-w.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ezu.sjlbkw.cn

[R11] case 多分支
来源：http://oua.ppjwa.cn

case "$1" in
来源：http://gnm.xinyue.icu

start) echo "启动" ;;
来源：http://lzm.vehdjk.com

stop)  echo "停止" ;;
来源：http://dxl.iojbl.cn

*)     echo "未知命令" ;;
来源：http://qzk.daxiang520.top

esac
来源：http://kpb.meibo888.top

[R12] for 遍历文件
来源：http://eid.xuetiantiany.cn

for f in *.txt; do echo "$f"; done
来源：http://mqh.yj202588.top

[R13] for 计数循环
来源：http://ich.wangdashe.top

for i in {1..10}; do echo "$i"; done
来源：http://oxj.zhiwuduotai.top

[R14] C 风格 for
来源：http://qdg.shuidangran.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sdv.ybcxt.top

[R15] while 逐行读文件
来源：http://ica.epnwcf.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zxm.shzxlz.cn

[R16] until 等待条件
来源：http://qad.nwbrower.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rxt.jianghu66.top

[R17] 数组定义与取值
来源：http://yjw.ctjpmb.com

arr=(a b c); echo "${arr[0]}"
来源：http://wbk.ybcxt.top

[R18] 遍历数组
来源：http://gff.shuidangran.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xiu.yangfankeji.com

[R19] 数组长度
来源：http://dwe.cqqwz.cn

echo "${#arr[@]}"
来源：http://flk.jianghu66.top

[R20] 关联数组（字典）
来源：http://zdo.xuanzx.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://znh.52xcode.cn

[R21] 字符串长度
来源：http://hkz.zhengqikj.top

echo "${#s}"
来源：http://oqx.chenlongwang.top

[R22] 截取子串
来源：http://vsl.jlsjyb.cn

echo "${s:0:5}"
来源：http://moc.daria6918.cn

[R23] 字符串替换
来源：http://cxs.meibo888.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yly.zhoulong.xyz

[R24] 大小写转换
来源：http://usb.iojbl.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lqh.zhiwuduotai.top

[R25] 去后缀 / 去前缀
来源：http://wyz.dianchejie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vfl.ybcxt.top

[R26] 命令替换
来源：http://fiv.hysaishi.cn

now=$(date +%F); echo "$now"
来源：http://ctf.tanke756.top

[R27] 算术展开
来源：http://kqf.hesvh.cn

echo $((1 + 2 * 3))
来源：http://qcu.jqgufenzy.top

[R28] 浮点运算
来源：http://lce.hysaishi.cn

echo "scale=2; 10/3" | bc
来源：http://lyb.ehwqpu.com

[R29] 定义函数
来源：http://lwu.jqgfzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vkm.zdbjq.cn

[R30] 函数返回状态码
来源：http://mml.sysykeji.top

f() { return 0; }; f || echo "失败了"
来源：http://rzx.nanxuanxn.top

[R31] 局部变量
来源：http://cgp.jianghu66.top

f() { local x=1; echo "$x"; }
来源：http://nzp.gaohongyu789.top

[R32] 参数个数校验
来源：http://wxh.haohaochexian.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tjp.bbcook.cn

[R33] 捕获错误并提示行号
来源：http://hkp.haohaochexian.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cua.yuxming.cn

[R34] 退出时清理
来源：http://htw.gzhubu.top

trap 'rm -f "$tmp"' EXIT
来源：http://jab.jinqigfzy.top

[R35] 后台执行并等待
来源：http://oyq.havefunace.top

sleep 5 & pid=$!; wait "$pid"
来源：http://gds.gogol.net.cn

[R36] 并发执行多个任务
来源：http://xpg.gogol.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fty.zdqjudy.top

[R37] 把输出赋给变量
来源：http://ime.fengsongda.top

files=$(ls -1)
来源：http://kjs.dashuyun.cn

[R38] 管道串联
来源：http://yoq.jinghuilouyu.cn

cat a.txt | grep -i error | wc -l
来源：http://lzv.sxryk.cn

[R39] 重定向标准输出与错误
来源：http://jvs.yueranfly.top

cmd > out.log 2>&1
来源：http://tng.fehbvm.com

[R40] 追加写日志
来源：http://not.xuanzx.com

echo "log" >> out.log
来源：http://ojf.bjfxy.top

[R41] 丢弃输出
来源：http://yls.ybcxt.top

cmd >/dev/null 2>&1
来源：http://yyt.chenjidiqi.icu

[R42] 输入重定向
来源：http://wrg.xziqi.cn

wc -l < a.txt
来源：http://mkv.hnxiangtu.top

[R43] 按名字查找文件
来源：http://sey.yongpay.top

find . -name "*.log" -type f
来源：http://biy.svipenyu.cn

[R44] 按修改时间查找
来源：http://ops.shanyushiyangtech.top

find . -mtime -7 -type f
来源：http://ars.ppjwa.cn

[R45] 批量删除
来源：http://gbx.daria6918.cn

find . -name "*.tmp" -delete
来源：http://mub.yuanzhike.top

[R46] 递归替换文件内容
来源：http://ywe.jqgfzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nnm.dashuyun.cn

[R47] sed 单行替换
来源：http://eqh.snrcjt.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sol.ydzc1.top

[R48] awk 取指定列
来源：http://bbv.52xcode.cn

awk '{print $1, $3}' a.txt
来源：http://zhp.yangfankeji.com

[R49] awk 带条件
来源：http://mli.shanyushiyangkeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lil.fzhhl.top

[R50] awk 求和
来源：http://vkt.shuidangran.top

awk '{s += $2} END {print s}' a.txt
来源：http://ijo.yj20258.top

[R51] 排序去重取前几
来源：http://iox.bbcook.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://uke.yangfankeji.com

[R52] 统计行数
来源：http://olj.yonumen.top

wc -l a.txt
来源：http://xwe.ctjpmb.com

[R53] 查看文件头与实时尾
来源：http://fpt.jqgufenzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dmy.yongpay.top

[R54] 比较两个文件
来源：http://lvm.xuanzx.com

diff a.txt b.txt
来源：http://tdm.cheryme.top

[R55] 压缩与解压
来源：http://fxx.xziqi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://esr.yvedp.cn

[R56] 远程拷贝
来源：http://tqz.uphjek.com

scp file user@host:/path/
来源：http://tul.yj20258.top

[R57] 远程执行命令
来源：http://zas.iojbl.cn

ssh user@host 'uptime'
来源：http://ddt.chenjidiqi.icu

[R58] 下载文件
来源：http://nly.yangfankeji.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uih.jqgufenzy.top

[R59] 发 POST JSON
来源：http://hmz.ivvv.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rqk.xinyue.icu

[R60] 只看 HTTP 状态码
来源：http://das.gotoacloud.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://far.yanxiufei.cn

[R61] 磁盘占用
来源：http://vqf.tian-w.cn

df -h;  du -sh *
来源：http://iij.shuidangran.top

[R62] 找最占空间的文件
来源：http://jyg.hcnkem.com

du -ah . | sort -rh | head -10
来源：http://fgi.zhongyouzk.top

[R63] 内存与进程
来源：http://jfv.gaohongyu789.top

free -h;  ps aux | grep nginx
来源：http://xdo.ivvv.top

[R64] 结束进程
来源：http://hjo.yuxming.cn

kill -9 $(pgrep -f app.py)
来源：http://rnj.9152youxi.cn

[R65] 查看端口占用
来源：http://mau.nanxinkj.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qck.snrcjt.cn

[R66] 定时任务
来源：http://fvn.hammf.cn

crontab -e;  crontab -l
来源：http://cne.daria6918.cn

[R67] 生成随机十六进制串
来源：http://svp.hysaishi.cn


<!-- 参考信息 -->