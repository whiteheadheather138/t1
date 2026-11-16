代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://aty.redwolf501.top

[Q20] IN 列表
来源：http://nwk.yongpay.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://glb.ydzc1.top

[Q21] 空值判断
来源：http://nxh.hcnkem.com

SELECT * FROM users WHERE email IS NULL;
来源：http://cxn.nwbrower.top

[Q22] 排序
来源：http://dcq.xingfuxueyuan.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dka.hysaishi.cn

[Q23] 分页
来源：http://czb.xinyue.icu

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fmf.xuetiantiany.cn

[Q24] 去重
来源：http://oez.guowangkeji.top

SELECT DISTINCT city FROM users;
来源：http://jxj.yanxiufei.cn

[Q25] 只取前 N 条
来源：http://uzd.zycfv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://shs.kuanghao11.cn

[Q26] 计数
来源：http://xhs.aibaodan.cn

SELECT COUNT(*) FROM users;
来源：http://pbe.aibaodan.cn

[Q27] 条件计数
来源：http://kzr.gotoacloud.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dvv.yj20258888.top

[Q28] 求和与平均
来源：http://mif.sjlbkw.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vla.tianlin.xyz

[Q29] 最大最小值
来源：http://rsj.yueranfly.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://mkl.birdmap.top

[Q30] 分组统计
来源：http://vxl.xuanzx.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yvy.fengsongda.top

[Q31] 分组后过滤
来源：http://cdl.ybcxt.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jco.ctjpmb.com

[Q32] 分组拼接字符串
来源：http://lde.zhiwuduotai.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://msr.jinqigfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://def.mhx1999.top

[Q33] 多列分组
来源：http://whw.snrcjt.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hjs.yj20258888.top

[Q34] 每组取第一条
来源：http://qge.pycfn.com

SELECT * FROM (
来源：http://usm.sjlbkw.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jjj.haohaochexian.top

) t WHERE rn = 1;
来源：http://mco.fktsv.cn

[Q35] 内连接
来源：http://wva.bbcook.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ekt.fanxiaobao.xyz

[Q36] 左连接
来源：http://vjr.ydzc1.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ndb.cdnleiting.top

[Q37] 右连接
来源：http://uwg.birdmap.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wod.yfazqb.com

[Q38] 全外连接（PostgreSQL）
来源：http://kyk.ctjpmb.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wuz.andypj.xyz

[Q39] 自连接（查上下级）
来源：http://kar.zhiwuduotai.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rcx.birdmap.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yko.gogol.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sgh.meibo888.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://abn.zhaomingkeji.xyz

[Q41] 多表连接
来源：http://djj.vehdjk.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://dxa.9152youxi.cn

JOIN users u ON u.id = o.user_id
来源：http://xkp.cheryme.top

JOIN products p ON p.id = o.product_id;
来源：http://xuc.sxryk.cn

[Q42] 连接条件附加过滤
来源：http://mlt.ppjwa.cn

SELECT u.name, o.amount FROM users u
来源：http://rqg.hongshengwenyu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ram.jiagoushi.top

[Q43] 标量子查询
来源：http://jts.quarkkingdee.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wpt.shzxlz.cn

[Q44] IN 子查询
来源：http://eej.0kj1m.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nxf.zdbjq.cn

[Q45] EXISTS 判断存在
来源：http://wni.ybcxt.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sgn.hongshengwenyu.top

[Q46] NOT EXISTS 判断不存在
来源：http://czz.yonumen.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dzt.sufxvd.cn

[Q47] 与平均值比较
来源：http://uok.bbcook.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dgn.xuanzx.com

[Q48] CTE 公用表表达式
来源：http://mno.gaohongyu789.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wpk.fehbvm.com

SELECT * FROM t WHERE c > 5;
来源：http://cda.cashguo.top

[Q49] 更新单行
来源：http://atg.epnwcf.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ivx.gotoacloud.top

[Q50] 批量更新
来源：http://rxi.hammf.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://aik.zhoulong.xyz

[Q51] 用子查询更新
来源：http://lkz.ydjk.org.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://aak.tanke756.top

[Q52] 删除指定行
来源：http://ujx.zdbjq.cn

DELETE FROM users WHERE id = 10;
来源：http://awy.zhiwuduotai.top

[Q53] 按条件删除
来源：http://ppe.guowangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xdg.cqqwz.cn

[Q54] 清空表
来源：http://kvk.xuetiantiany.cn

TRUNCATE TABLE logs;
来源：http://cur.xuanzx.com

[Q55] 排名（并列占位）
来源：http://mgx.ivvv.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://iey.meibo888.top

[Q56] 密集排名（并列不占位）
来源：http://oeo.gogol.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sos.9152youxi.cn

[Q57] 行号
来源：http://xwv.xuanzx.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eds.jqgfzy.top

[Q58] 累计求和
来源：http://zsj.sysykeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lgn.xziqi.cn

[Q59] 分组内累计
来源：http://yad.aizwys.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xbv.jqgfzy.top

[Q60] 取上一行 / 下一行
来源：http://ocr.zhoulong.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nqc.zhijiandao.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wvi.ctjpmb.com

[Q61] 移动平均
来源：http://jfj.yj202588.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wpw.zhengqikj.top

[Q62] 分组占比
来源：http://rxr.shuidangran.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://obq.xuanzx.com

[Q63] 开启事务
来源：http://tzl.redwolf501.top

START TRANSACTION;                -- 或 BEGIN
来源：http://osw.gotoacloud.top

[Q64] 提交事务
来源：http://byv.gotoacloud.top

COMMIT;
来源：http://cnb.bjfxy.top

[Q65] 回滚事务
来源：http://txz.nanxuanxn.top

ROLLBACK;
来源：http://eiv.jiagoushi.top

[Q66] 行锁查询
来源：http://llq.ivvv.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mnt.fehbvm.com

[Q67] 设置隔离级别
来源：http://vzz.wangshuangyany.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xra.uphjek.com

[Q68] 保存点
来源：http://pgy.gaohongyu789.top

SAVEPOINT sp1;
来源：http://qlr.xylfe.cn

ROLLBACK TO sp1;
来源：http://qbn.zhoulong.xyz

[Q69] 查看执行计划
来源：http://fug.shanyushiyangkeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://szq.shanyushiyangkeji.top

[Q70] 更新统计信息
来源：http://sfb.jinqigfzy.top

ANALYZE TABLE users;
来源：http://vlv.bbcook.cn

[Q71] 查看建表语句
来源：http://mdg.vehdjk.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hik.jiagoushi.top

[Q72] 查看索引
来源：http://qnf.jiagoushi.top

SHOW INDEX FROM users;
来源：http://nhy.feifeiyinyue.top

[Q73] 查看表状态
来源：http://ymk.0kj1m.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zic.tian-w.cn

[Q74] 强制使用索引
来源：http://jrs.fzhhl.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uzx.sweek.top

[Q75] 日期格式化
来源：http://rpw.zycfv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fqi.shanyushiyangtech.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gob.feifeiyinyue.top

[Q76] 按天统计
来源：http://xjn.nwbrower.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dwm.xinyue.icu

[Q77] 时间加减
来源：http://cvd.zhiwuduotai.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://aeb.gaohongyu789.top

[Q78] 当前时间
来源：http://pvy.sxryk.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ayn.sxryk.cn

[Q79] 字符串拼接
来源：http://lgj.hywenlv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iam.ydjk.org.cn

[Q80] 字符串截取
来源：http://evo.xylfe.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gjd.shanyushiyangtech.top

[Q81] 字符串替换
来源：http://yug.jqgfzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qbz.ybcxt.top

[Q82] 字符长度与字节长度
来源：http://ucf.jinghuilouyu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://spc.shanyushiyangkeji.top

[Q83] 大小写转换
来源：http://spt.meibo888.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jzy.sxryk.cn

[Q84] 去除首尾空格
来源：http://bsp.sweek.top

SELECT TRIM(name) FROM users;
来源：http://tso.yonumen.top

[Q85] 数值取整
来源：http://rrr.meibo888.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lgd.fengsongda.top

[Q86] 读取 JSON 字段
来源：http://byp.jianghu66.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://aqo.sysykeji.top

[Q87] JSON 字段做条件
来源：http://zdw.yuanzhike.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eol.dashuyun.cn

[Q88] 行转列（条件聚合）
来源：http://fza.jinqigfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yhy.shanyushiyangtech.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tda.pengpengdd.cyou

[Q89] 判断表是否存在
来源：http://zsl.yonumen.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vnm.tarul.cn

[Q90] 生成序号列
来源：http://tfk.xylfe.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mxu.jinqigufen.top

================================================================================
来源：http://tkd.jinghuilouyu.cn

R. Bash 专题
来源：http://jlo.gaohongyu789.top

================================================================================
来源：http://pmu.jlsjyb.cn

[R01] shebang 与严格模式
来源：http://zoy.hesvh.cn

#!/usr/bin/env bash
来源：http://qza.xingfuxueyuan.xyz

set -euo pipefail
来源：http://jrx.havefunace.top

[R02] 变量赋值与使用
来源：http://oik.0kj1m.cn

name="Tom"; echo "$name"
来源：http://hiu.pengpengdd.cyou

[R03] 只读变量
来源：http://tmm.tanke756.top

readonly PI=3.14
来源：http://owx.tian-w.cn

[R04] 位置参数
来源：http://zrf.xziqi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eyp.tian-w.cn

[R05] 参数默认值
来源：http://vxq.gotoacloud.top

name="${1:-default}"
来源：http://cdy.cucudq.cn

[R06] 判断命令是否存在
来源：http://tqu.bbcook.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gnr.xylfe.cn

[R07] if 判断文件
来源：http://etp.vqdsnc.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dmv.zhixingplan.top

[R08] 数值比较
来源：http://reo.fehbvm.com

if (( a > b )); then echo "a 更大"; fi
来源：http://hgy.zdqjudy.top

[R09] 字符串比较
来源：http://ast.c1oappe.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wuz.yfazqb.com

[R10] 正则匹配
来源：http://ieu.bbcook.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jrn.zhijiandao.cn

[R11] case 多分支
来源：http://nii.guowangkeji.top

case "$1" in
来源：http://tkd.smart0.xyz

start) echo "启动" ;;
来源：http://tbk.gzhubu.top

stop)  echo "停止" ;;
来源：http://pgz.tarul.cn

*)     echo "未知命令" ;;
来源：http://rzg.yj20258.top

esac
来源：http://aet.sysykeji.top

[R12] for 遍历文件
来源：http://wmm.feifeiyinyue.top

for f in *.txt; do echo "$f"; done
来源：http://kzd.yj20258.top

[R13] for 计数循环
来源：http://drf.ywan-chungtsiang.top

for i in {1..10}; do echo "$i"; done
来源：http://she.sweek.top

[R14] C 风格 for
来源：http://ewn.quarkkingdee.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://izi.vehdjk.com

[R15] while 逐行读文件
来源：http://ims.dashuyun.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ldh.xylfe.cn

[R16] until 等待条件
来源：http://qpi.yangfankeji.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xec.haohaochexian.top

[R17] 数组定义与取值
来源：http://zxi.fktsv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jms.yvedp.cn

[R18] 遍历数组
来源：http://qvz.svipenyu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nnx.epnwcf.com

[R19] 数组长度
来源：http://lti.ywan-chungtsiang.top

echo "${#arr[@]}"
来源：http://wog.bjfxy.top

[R20] 关联数组（字典）
来源：http://wwc.zhiwuduotai.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hik.yuanzhike.top

[R21] 字符串长度
来源：http://xne.hcnkem.com

echo "${#s}"
来源：http://jyr.daria6918.cn

[R22] 截取子串
来源：http://hne.xylfe.cn

echo "${s:0:5}"
来源：http://msq.dianchejie.cn

[R23] 字符串替换
来源：http://jjk.bbcook.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qgr.meibo888.top

[R24] 大小写转换
来源：http://vin.yj20258.top

echo "${s^^}"; echo "${s,,}"
来源：http://vrp.shzxlz.cn

[R25] 去后缀 / 去前缀
来源：http://ovk.sjlbkw.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://roh.chenzaomai.com

[R26] 命令替换
来源：http://ndg.yuxming.cn

now=$(date +%F); echo "$now"
来源：http://erm.yongpay.top

[R27] 算术展开
来源：http://gtv.ivvv.top

echo $((1 + 2 * 3))
来源：http://dyr.bbcook.cn

[R28] 浮点运算
来源：http://euv.xylfe.cn

echo "scale=2; 10/3" | bc
来源：http://hil.smart0.xyz

[R29] 定义函数
来源：http://vzs.svipenyu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qty.shanyushiyangtech.top

[R30] 函数返回状态码
来源：http://ydn.tian-w.cn

f() { return 0; }; f || echo "失败了"
来源：http://npu.zhijiandao.cn

[R31] 局部变量
来源：http://lrp.yj202588.top

f() { local x=1; echo "$x"; }
来源：http://jxn.yongpay.top

[R32] 参数个数校验
来源：http://upn.jqgufenzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sgi.haohaochexian.top

[R33] 捕获错误并提示行号
来源：http://mbu.wangshuangyany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fta.mhx1999.top

[R34] 退出时清理
来源：http://tpx.hongshengwenyu.top

trap 'rm -f "$tmp"' EXIT
来源：http://xny.ydjk.org.cn

[R35] 后台执行并等待
来源：http://pmi.sxryk.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ywu.xingfuxueyuan.xyz

[R36] 并发执行多个任务
来源：http://rve.feifeiyinyue.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fry.bjfxy.top

[R37] 把输出赋给变量
来源：http://vfj.sysykeji.top

files=$(ls -1)
来源：http://hqj.cashguo.top

[R38] 管道串联
来源：http://ulu.yuxming.cn

cat a.txt | grep -i error | wc -l
来源：http://vzf.shzxlz.cn

[R39] 重定向标准输出与错误
来源：http://gph.chenjidiqi.icu

cmd > out.log 2>&1
来源：http://fxb.316326.xyz

[R40] 追加写日志
来源：http://yql.hnqzz.top

echo "log" >> out.log
来源：http://ocg.c1oappe.top

[R41] 丢弃输出
来源：http://raz.tian-w.cn

cmd >/dev/null 2>&1
来源：http://ses.birdmap.top

[R42] 输入重定向
来源：http://gpe.316326.xyz

wc -l < a.txt
来源：http://jqy.smart0.xyz

[R43] 按名字查找文件
来源：http://gil.yj20258.top

find . -name "*.log" -type f
来源：http://mrx.cdnleiting.top

[R44] 按修改时间查找
来源：http://bin.ybcxt.top

find . -mtime -7 -type f
来源：http://brs.cucudq.cn

[R45] 批量删除
来源：http://gny.pycfn.com

find . -name "*.tmp" -delete
来源：http://yzd.guannengcc.top

[R46] 递归替换文件内容
来源：http://dhv.ywan-chungtsiang.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wio.fengsongda.top

[R47] sed 单行替换
来源：http://myi.sweek.top

sed -i 's/foo/bar/g' a.txt
来源：http://vnu.zdqjudy.top

[R48] awk 取指定列
来源：http://fyy.gaohongyu789.top

awk '{print $1, $3}' a.txt
来源：http://uqb.pengpengdd.cyou

[R49] awk 带条件
来源：http://meu.yanxiufei.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://otf.wangshuangyany.cn

[R50] awk 求和
来源：http://ndz.svipenyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sbo.ehwqpu.com

[R51] 排序去重取前几
来源：http://jah.xingfuxueyuan.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://xmp.tian-w.cn

[R52] 统计行数
来源：http://fdg.316326.xyz

wc -l a.txt
来源：http://gar.nanxuanxn.top

[R53] 查看文件头与实时尾
来源：http://znc.yuanzhike.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rjw.yangfankeji.com

[R54] 比较两个文件
来源：http://ktx.shanyushiyangkeji.top

diff a.txt b.txt
来源：http://iur.hnxiangtu.top

[R55] 压缩与解压
来源：http://eem.aizwys.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://oqy.sysykeji.top

[R56] 远程拷贝
来源：http://ymf.xuetiantiany.cn

scp file user@host:/path/
来源：http://puv.shangyingyoupin.top

[R57] 远程执行命令
来源：http://rxk.nwbrower.top

ssh user@host 'uptime'
来源：http://tyn.redwolf501.top

[R58] 下载文件
来源：http://fww.sufxvd.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wff.hnqzz.top

[R59] 发 POST JSON
来源：http://wbu.xylfe.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xoz.xylfe.cn

[R60] 只看 HTTP 状态码
来源：http://qov.ydjk.org.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xfd.bjfxy.top

[R61] 磁盘占用
来源：http://fdd.birdmap.top

df -h;  du -sh *
来源：http://rzd.xylfe.cn

[R62] 找最占空间的文件
来源：http://pmt.hammf.cn

du -ah . | sort -rh | head -10
来源：http://ous.cucudq.cn

[R63] 内存与进程
来源：http://lwn.fehbvm.com

free -h;  ps aux | grep nginx
来源：http://tqj.ydzc1.top

[R64] 结束进程
来源：http://pmz.yuxming.cn

kill -9 $(pgrep -f app.py)
来源：http://rro.zhoulong.xyz

[R65] 查看端口占用
来源：http://kyv.cdnleiting.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://egm.ppjwa.cn

[R66] 定时任务
来源：http://afs.jinyuanbaomall.cn

crontab -e;  crontab -l
来源：http://ijp.xziqi.cn

[R67] 生成随机十六进制串
来源：http://ztl.yvedp.cn

openssl rand -hex 16
来源：http://zmi.yangfankeji.com

[R68] 计算文件校验值
来源：http://qbi.jqgufenzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://kxm.daria6918.cn

[R69] 生成随机密码
来源：http://ihe.jyoumei.cn


<!-- 参考信息 -->