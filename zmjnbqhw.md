代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://miz.yj20258888.top

[Q18] 模糊匹配
来源：http://vjp.hongshengwenyu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qbg.shangyingyoupin.top

[Q19] 范围查询
来源：http://kgp.chenjidiqi.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oct.hnqzz.top

[Q20] IN 列表
来源：http://kxt.jlsjyb.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ueh.vqdsnc.cn

[Q21] 空值判断
来源：http://jej.xingfuxueyuan.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://dkd.gaohongyu789.top

[Q22] 排序
来源：http://tjh.nwbrower.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://smw.guannengcc.top

[Q23] 分页
来源：http://doc.svipenyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rsm.daxiang520.top

[Q24] 去重
来源：http://hwg.zhengqikj.top

SELECT DISTINCT city FROM users;
来源：http://grc.andypj.xyz

[Q25] 只取前 N 条
来源：http://qas.pycfn.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gph.guowangkeji.top

[Q26] 计数
来源：http://cmz.yanxiufei.cn

SELECT COUNT(*) FROM users;
来源：http://cgx.fktsv.cn

[Q27] 条件计数
来源：http://olr.gaohongyu789.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sfv.gaohongyu789.top

[Q28] 求和与平均
来源：http://fuz.jinyuanbaomall.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oyl.pycfn.com

[Q29] 最大最小值
来源：http://eem.yj202588.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://myl.nanxinkj.top

[Q30] 分组统计
来源：http://tdb.sweek.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gak.tianlin.xyz

[Q31] 分组后过滤
来源：http://wak.wangshuangyany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jtf.ivvv.top

[Q32] 分组拼接字符串
来源：http://laf.chenjidiqi.icu

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bmn.xuanzx.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fbp.ivvv.top

[Q33] 多列分组
来源：http://skz.tian-w.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yet.zhongyouzk.top

[Q34] 每组取第一条
来源：http://yrg.svipenyu.cn

SELECT * FROM (
来源：http://bro.nanxinkj.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://eai.yangfankeji.com

) t WHERE rn = 1;
来源：http://tzf.ydjk.org.cn

[Q35] 内连接
来源：http://clf.cdnleiting.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gxc.sufxvd.cn

[Q36] 左连接
来源：http://fxq.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vss.vehdjk.com

[Q37] 右连接
来源：http://lpx.fanxiaobao.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://avy.guowangkeji.top

[Q38] 全外连接（PostgreSQL）
来源：http://usg.hammf.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lvh.yuxming.cn

[Q39] 自连接（查上下级）
来源：http://mki.hnqzz.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ihq.feifeiyinyue.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tuz.shuidangran.top

[Q40] 交叉连接（笛卡尔积）
来源：http://itb.jinghuilouyu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uga.ivvv.top

[Q41] 多表连接
来源：http://gjn.guowangkeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bxl.guannengcc.top

JOIN users u ON u.id = o.user_id
来源：http://jpv.hesvh.cn

JOIN products p ON p.id = o.product_id;
来源：http://qku.shangyingyoupin.top

[Q42] 连接条件附加过滤
来源：http://fxa.ivvv.top

SELECT u.name, o.amount FROM users u
来源：http://muy.aibaodan.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://anl.daria6918.cn

[Q43] 标量子查询
来源：http://nre.cheryme.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://izz.gaohongyu789.top

[Q44] IN 子查询
来源：http://qrf.fzhhl.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vbv.hnqzz.top

[Q45] EXISTS 判断存在
来源：http://hkw.zdqjudy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qpl.redwolf501.top

[Q46] NOT EXISTS 判断不存在
来源：http://plf.yfazqb.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fvh.xuetiantiany.cn

[Q47] 与平均值比较
来源：http://elj.sweek.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://irm.fktsv.cn

[Q48] CTE 公用表表达式
来源：http://sno.jinqigfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fkj.xziqi.cn

SELECT * FROM t WHERE c > 5;
来源：http://xvu.cheryme.top

[Q49] 更新单行
来源：http://pgo.ybcxt.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mun.ydzc1.top

[Q50] 批量更新
来源：http://mbm.yvedp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cmb.316326.xyz

[Q51] 用子查询更新
来源：http://zpz.iojbl.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://chs.yvedp.cn

[Q52] 删除指定行
来源：http://afb.gaohongyu789.top

DELETE FROM users WHERE id = 10;
来源：http://flr.xylfe.cn

[Q53] 按条件删除
来源：http://rlb.sysykeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rfo.daria6918.cn

[Q54] 清空表
来源：http://zqq.feifeiyinyue.top

TRUNCATE TABLE logs;
来源：http://zup.kuanghao11.cn

[Q55] 排名（并列占位）
来源：http://ksk.shzxlz.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vze.daxiang520.top

[Q56] 密集排名（并列不占位）
来源：http://cet.fanxiaobao.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qjw.ivvv.top

[Q57] 行号
来源：http://isc.epnwcf.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cag.fengsongda.top

[Q58] 累计求和
来源：http://pfh.9152youxi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://udk.0kj1m.cn

[Q59] 分组内累计
来源：http://cej.smart0.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ima.jlsjyb.cn

[Q60] 取上一行 / 下一行
来源：http://dpq.ydzc1.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ner.epnwcf.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ngk.yuxming.cn

[Q61] 移动平均
来源：http://gev.ybcxt.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://siq.hfpthk.cn

[Q62] 分组占比
来源：http://xhl.shzxlz.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xrh.uphjek.com

[Q63] 开启事务
来源：http://ijs.nanxinkj.top

START TRANSACTION;                -- 或 BEGIN
来源：http://aei.yonumen.top

[Q64] 提交事务
来源：http://upk.daxiang520.top

COMMIT;
来源：http://fko.hesvh.cn

[Q65] 回滚事务
来源：http://idf.hywenlv.cn

ROLLBACK;
来源：http://axi.yuanzhike.top

[Q66] 行锁查询
来源：http://ktj.hnxiangtu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mfm.xylfe.cn

[Q67] 设置隔离级别
来源：http://lcl.tarul.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sdo.9152youxi.cn

[Q68] 保存点
来源：http://qpr.redwolf501.top

SAVEPOINT sp1;
来源：http://his.cashguo.top

ROLLBACK TO sp1;
来源：http://xpu.sufxvd.cn

[Q69] 查看执行计划
来源：http://xnm.fktsv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mjq.ywan-chungtsiang.top

[Q70] 更新统计信息
来源：http://xlh.dianchejie.cn

ANALYZE TABLE users;
来源：http://rsr.jiagoushi.top

[Q71] 查看建表语句
来源：http://vcz.wangshuangyany.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mov.bjfxy.top

[Q72] 查看索引
来源：http://pws.jiagoushi.top

SHOW INDEX FROM users;
来源：http://gle.birdmap.top

[Q73] 查看表状态
来源：http://vxa.xinyue.icu

SHOW TABLE STATUS LIKE 'users';
来源：http://opc.jqgfzy.top

[Q74] 强制使用索引
来源：http://siw.xinyue.icu

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sqj.zdbjq.cn

[Q75] 日期格式化
来源：http://lqi.wangshuangyany.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xnd.dianchejie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ggw.yuxming.cn

[Q76] 按天统计
来源：http://gnq.tian-w.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://irk.yj20258888.top

[Q77] 时间加减
来源：http://lzf.yj20258.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cjh.0kj1m.cn

[Q78] 当前时间
来源：http://vzp.hfpthk.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bwu.xinyue.icu

[Q79] 字符串拼接
来源：http://qst.snrcjt.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hrl.hfpthk.cn

[Q80] 字符串截取
来源：http://gbi.shanyushiyangtech.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pif.hongshengwenyu.top

[Q81] 字符串替换
来源：http://vco.daria6918.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mic.xingfuxueyuan.xyz

[Q82] 字符长度与字节长度
来源：http://uwt.vehdjk.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xih.nanxinkj.top

[Q83] 大小写转换
来源：http://prb.zhaomingkeji.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dix.ctjpmb.com

[Q84] 去除首尾空格
来源：http://kpa.daxiang520.top

SELECT TRIM(name) FROM users;
来源：http://oxq.xziqi.cn

[Q85] 数值取整
来源：http://uqe.xinyue.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yeg.jqgufenzy.top

[Q86] 读取 JSON 字段
来源：http://voh.tianlin.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qrd.shuidangran.top

[Q87] JSON 字段做条件
来源：http://vjb.gotoacloud.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mon.guannengcc.top

[Q88] 行转列（条件聚合）
来源：http://zgr.gogol.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rue.guannengcc.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ido.tianlin.xyz

[Q89] 判断表是否存在
来源：http://zav.yangfankeji.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dto.316326.xyz

[Q90] 生成序号列
来源：http://gpa.zhaomingkeji.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ssr.hesvh.cn

================================================================================
来源：http://igz.hammf.cn

R. Bash 专题
来源：http://ypk.hammf.cn

================================================================================
来源：http://cre.hnqzz.top

[R01] shebang 与严格模式
来源：http://rdp.smart0.xyz

#!/usr/bin/env bash
来源：http://dpu.chenlongwang.top

set -euo pipefail
来源：http://mob.shangyingyoupin.top

[R02] 变量赋值与使用
来源：http://vvn.cheryme.top

name="Tom"; echo "$name"
来源：http://dpg.nwbrower.top

[R03] 只读变量
来源：http://ozk.ivvv.top

readonly PI=3.14
来源：http://zce.shanyushiyangtech.top

[R04] 位置参数
来源：http://kkh.vehdjk.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cjk.ydjk.org.cn

[R05] 参数默认值
来源：http://svr.jinqigufen.top

name="${1:-default}"
来源：http://sct.jqgufenzy.top

[R06] 判断命令是否存在
来源：http://ypr.ybcxt.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://osl.hnqzz.top

[R07] if 判断文件
来源：http://btz.sufxvd.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yvj.zhoulong.xyz

[R08] 数值比较
来源：http://mku.xuetiantiany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zmx.xinyue.icu

[R09] 字符串比较
来源：http://xgi.wangshuangyany.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rue.fanxiaobao.xyz

[R10] 正则匹配
来源：http://xgv.iojbl.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cri.sxryk.cn

[R11] case 多分支
来源：http://ntr.andypj.xyz

case "$1" in
来源：http://crq.dianchejie.cn

start) echo "启动" ;;
来源：http://twm.birdmap.top

stop)  echo "停止" ;;
来源：http://ygl.smart0.xyz

*)     echo "未知命令" ;;
来源：http://pmg.fengsongda.top

esac
来源：http://yek.quarkkingdee.top

[R12] for 遍历文件
来源：http://wht.0kj1m.cn

for f in *.txt; do echo "$f"; done
来源：http://rqv.nwbrower.top

[R13] for 计数循环
来源：http://xeb.jqgufenzy.top

for i in {1..10}; do echo "$i"; done
来源：http://qwx.gogol.net.cn

[R14] C 风格 for
来源：http://pop.ydzc1.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bwy.cdnleiting.top

[R15] while 逐行读文件
来源：http://lhb.wangshuangyany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zsy.xuanzx.com

[R16] until 等待条件
来源：http://gjk.jlsjyb.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hdj.zhaomingkeji.xyz

[R17] 数组定义与取值
来源：http://wps.aizwys.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hmf.tanke756.top

[R18] 遍历数组
来源：http://ksu.gzhubu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bbc.shanyushiyangtech.top

[R19] 数组长度
来源：http://qff.sweek.top

echo "${#arr[@]}"
来源：http://squ.zycfv.cn

[R20] 关联数组（字典）
来源：http://oku.hesvh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vck.zhongyouzk.top

[R21] 字符串长度
来源：http://nzq.nanxinkj.top

echo "${#s}"
来源：http://fpj.zdbjq.cn

[R22] 截取子串
来源：http://msh.9152youxi.cn

echo "${s:0:5}"
来源：http://jau.aibaodan.cn

[R23] 字符串替换
来源：http://oun.svipenyu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vnq.cdnleiting.top

[R24] 大小写转换
来源：http://ntn.daria6918.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mpu.yanxiufei.cn

[R25] 去后缀 / 去前缀
来源：http://vay.daxiang520.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://aws.meibo888.top

[R26] 命令替换
来源：http://poy.hnqzz.top

now=$(date +%F); echo "$now"
来源：http://trl.vqdsnc.cn

[R27] 算术展开
来源：http://unn.yuanzhike.top

echo $((1 + 2 * 3))
来源：http://zxt.sxryk.cn

[R28] 浮点运算
来源：http://fjj.birdmap.top

echo "scale=2; 10/3" | bc
来源：http://krn.nanxinkj.top

[R29] 定义函数
来源：http://hqf.tarul.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sof.daxiang520.top

[R30] 函数返回状态码
来源：http://bek.gzhubu.top

f() { return 0; }; f || echo "失败了"
来源：http://dtm.hesvh.cn

[R31] 局部变量
来源：http://wht.jyoumei.cn

f() { local x=1; echo "$x"; }
来源：http://wcw.snrcjt.cn

[R32] 参数个数校验
来源：http://pxq.hfpthk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ksk.jinyuanbaomall.cn

[R33] 捕获错误并提示行号
来源：http://poq.snrcjt.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mma.sysykeji.top

[R34] 退出时清理
来源：http://ril.shzxlz.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hup.jinghuilouyu.cn

[R35] 后台执行并等待
来源：http://qdi.xziqi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ipv.gogol.net.cn

[R36] 并发执行多个任务
来源：http://rrv.vehdjk.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jxm.uphjek.com

[R37] 把输出赋给变量
来源：http://ajk.cheryme.top

files=$(ls -1)
来源：http://eim.xziqi.cn

[R38] 管道串联
来源：http://gii.fktsv.cn

cat a.txt | grep -i error | wc -l
来源：http://rnu.jlsjyb.cn

[R39] 重定向标准输出与错误
来源：http://vrd.yj202588.top

cmd > out.log 2>&1
来源：http://otu.jqgufenzy.top

[R40] 追加写日志
来源：http://sio.gogol.net.cn

echo "log" >> out.log
来源：http://wrh.hnqzz.top

[R41] 丢弃输出
来源：http://cdq.haohaochexian.top

cmd >/dev/null 2>&1
来源：http://ddv.yueranfly.top

[R42] 输入重定向
来源：http://ltk.daxiang520.top

wc -l < a.txt
来源：http://kxy.wangshuangyany.cn

[R43] 按名字查找文件
来源：http://rzn.jyoumei.cn

find . -name "*.log" -type f
来源：http://pkn.smart0.xyz

[R44] 按修改时间查找
来源：http://ybr.cucudq.cn

find . -mtime -7 -type f
来源：http://arv.hysaishi.cn

[R45] 批量删除
来源：http://qua.sjlbkw.cn

find . -name "*.tmp" -delete
来源：http://gfr.kuanghao11.cn

[R46] 递归替换文件内容
来源：http://spz.zdbjq.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://chk.zhongyouzk.top

[R47] sed 单行替换
来源：http://hxw.nanxinkj.top

sed -i 's/foo/bar/g' a.txt
来源：http://zcy.hysaishi.cn

[R48] awk 取指定列
来源：http://aet.uphjek.com

awk '{print $1, $3}' a.txt
来源：http://dzv.ydzc1.top

[R49] awk 带条件
来源：http://avl.sysykeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://eig.cucudq.cn

[R50] awk 求和
来源：http://nei.gotoacloud.top

awk '{s += $2} END {print s}' a.txt
来源：http://ted.cashguo.top

[R51] 排序去重取前几
来源：http://dwl.pycfn.com

sort a.txt | uniq -c | sort -rn | head
来源：http://rwv.nanxinkj.top

[R52] 统计行数
来源：http://sqx.kuanghao11.cn

wc -l a.txt
来源：http://qds.cdnleiting.top

[R53] 查看文件头与实时尾
来源：http://iri.yanxiufei.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pdc.cdnleiting.top

[R54] 比较两个文件
来源：http://nav.havefunace.top

diff a.txt b.txt
来源：http://srt.zhijiandao.cn

[R55] 压缩与解压
来源：http://jva.jiagoushi.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://egn.shangyingyoupin.top

[R56] 远程拷贝
来源：http://xlx.shanyushiyangtech.top

scp file user@host:/path/
来源：http://jwt.nanxinkj.top

[R57] 远程执行命令
来源：http://bhq.tianlin.xyz

ssh user@host 'uptime'
来源：http://ils.jyoumei.cn

[R58] 下载文件
来源：http://akw.hnqzz.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bkz.hysaishi.cn

[R59] 发 POST JSON
来源：http://yzv.zhijiandao.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://aof.redwolf501.top

[R60] 只看 HTTP 状态码
来源：http://bee.chenjidiqi.icu

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pve.daria6918.cn

[R61] 磁盘占用
来源：http://uri.fehbvm.com

df -h;  du -sh *
来源：http://zjm.zhijiandao.cn

[R62] 找最占空间的文件
来源：http://hcb.ydzc1.top

du -ah . | sort -rh | head -10
来源：http://pxk.cucudq.cn

[R63] 内存与进程
来源：http://vuu.sysykeji.top

free -h;  ps aux | grep nginx
来源：http://has.kuanghao11.cn

[R64] 结束进程
来源：http://sha.sysykeji.top

kill -9 $(pgrep -f app.py)
来源：http://dhc.yuanzhike.top

[R65] 查看端口占用
来源：http://zai.feifeiyinyue.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dmo.pengpengdd.cyou

[R66] 定时任务
来源：http://erp.cheryme.top

crontab -e;  crontab -l
来源：http://zgk.jianghu66.top

[R67] 生成随机十六进制串
来源：http://jig.cashguo.top


<!-- 参考信息 -->