代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://ypw.cheryme.top

[Q22] 排序
来源：http://muq.jinqigufen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ecr.svipenyu.cn

[Q23] 分页
来源：http://hro.gaohongyu789.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dbf.nanxinkj.top

[Q24] 去重
来源：http://ecr.sweek.top

SELECT DISTINCT city FROM users;
来源：http://mjj.ctjpmb.com

[Q25] 只取前 N 条
来源：http://oqq.zycfv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qlt.uphjek.com

[Q26] 计数
来源：http://qwi.yfazqb.com

SELECT COUNT(*) FROM users;
来源：http://xpc.gzhubu.top

[Q27] 条件计数
来源：http://cnn.pengpengdd.cyou

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fjc.andypj.xyz

[Q28] 求和与平均
来源：http://djd.yj20258.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://keu.zhiwuduotai.top

[Q29] 最大最小值
来源：http://ewq.52xcode.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://biz.jinyuanbaomall.cn

[Q30] 分组统计
来源：http://adz.zdqjudy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gkb.yj202588.top

[Q31] 分组后过滤
来源：http://mks.jqgfzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bft.ydzc1.top

[Q32] 分组拼接字符串
来源：http://ocd.yuxming.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vkb.daria6918.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://saz.vehdjk.com

[Q33] 多列分组
来源：http://lod.hfpthk.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tau.jinghuilouyu.cn

[Q34] 每组取第一条
来源：http://ril.yuxming.cn

SELECT * FROM (
来源：http://qhe.shangyingyoupin.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fxo.pengpengdd.cyou

) t WHERE rn = 1;
来源：http://otj.jlsjyb.cn

[Q35] 内连接
来源：http://ccz.hesvh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jrl.sweek.top

[Q36] 左连接
来源：http://ngb.shuidangran.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yxf.jianghu66.top

[Q37] 右连接
来源：http://uro.yueranfly.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pve.jqgufenzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://dfu.tarul.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tvq.gotoacloud.top

[Q39] 自连接（查上下级）
来源：http://vfq.zycfv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qpk.shzxlz.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ert.kuanghao11.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pbu.hongshengwenyu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://amo.fktsv.cn

[Q41] 多表连接
来源：http://scr.redwolf501.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://tld.hammf.cn

JOIN users u ON u.id = o.user_id
来源：http://kyr.c1oappe.top

JOIN products p ON p.id = o.product_id;
来源：http://nsx.havefunace.top

[Q42] 连接条件附加过滤
来源：http://ria.pengpengdd.cyou

SELECT u.name, o.amount FROM users u
来源：http://hss.shuidangran.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jpu.gaohongyu789.top

[Q43] 标量子查询
来源：http://yhn.gzhubu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://buc.quarkkingdee.top

[Q44] IN 子查询
来源：http://jup.zhongyouzk.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cob.hywenlv.cn

[Q45] EXISTS 判断存在
来源：http://kjt.yj20258.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://axs.zhixingplan.top

[Q46] NOT EXISTS 判断不存在
来源：http://hhp.gogol.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rnb.sysykeji.top

[Q47] 与平均值比较
来源：http://sum.zhongyouzk.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rim.aizwys.cn

[Q48] CTE 公用表表达式
来源：http://nvl.nanxuanxn.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kps.zhoulong.xyz

SELECT * FROM t WHERE c > 5;
来源：http://rmf.cqqwz.cn

[Q49] 更新单行
来源：http://jym.fktsv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hum.pengpengdd.cyou

[Q50] 批量更新
来源：http://evn.shanyushiyangtech.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hhl.shanyushiyangkeji.top

[Q51] 用子查询更新
来源：http://uhg.xuanzx.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://eae.shanyushiyangkeji.top

[Q52] 删除指定行
来源：http://tfi.hcnkem.com

DELETE FROM users WHERE id = 10;
来源：http://xag.xuanzx.com

[Q53] 按条件删除
来源：http://bvt.zhoulong.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rnb.daxiang520.top

[Q54] 清空表
来源：http://hgr.jianghu66.top

TRUNCATE TABLE logs;
来源：http://zvb.ppjwa.cn

[Q55] 排名（并列占位）
来源：http://lwa.svipenyu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kdo.316326.xyz

[Q56] 密集排名（并列不占位）
来源：http://yew.ydjk.org.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hwl.gotoacloud.top

[Q57] 行号
来源：http://sgz.daxiang520.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hbh.ydzc1.top

[Q58] 累计求和
来源：http://vrw.jyoumei.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qmr.fengsongda.top

[Q59] 分组内累计
来源：http://nlv.yj20258.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://exj.daria6918.cn

[Q60] 取上一行 / 下一行
来源：http://smo.guannengcc.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ooh.guannengcc.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ity.yfazqb.com

[Q61] 移动平均
来源：http://sje.shangyingyoupin.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hyk.xuanzx.com

[Q62] 分组占比
来源：http://ind.zhiwuduotai.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zpk.epnwcf.com

[Q63] 开启事务
来源：http://mrh.zdqjudy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://qcb.zhengqikj.top

[Q64] 提交事务
来源：http://dwe.pengpengdd.cyou

COMMIT;
来源：http://vfs.zhaomingkeji.xyz

[Q65] 回滚事务
来源：http://ryj.snrcjt.cn

ROLLBACK;
来源：http://abe.nanxuanxn.top

[Q66] 行锁查询
来源：http://hvd.zdbjq.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cnh.xuanzx.com

[Q67] 设置隔离级别
来源：http://fgj.cqqwz.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pfs.jiagoushi.top

[Q68] 保存点
来源：http://rdf.wangdashe.top

SAVEPOINT sp1;
来源：http://tgu.sxryk.cn

ROLLBACK TO sp1;
来源：http://ngm.yuanzhike.top

[Q69] 查看执行计划
来源：http://udm.dianchejie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://apk.cdnleiting.top

[Q70] 更新统计信息
来源：http://eta.yfazqb.com

ANALYZE TABLE users;
来源：http://tte.hysaishi.cn

[Q71] 查看建表语句
来源：http://bsp.ctjpmb.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yda.svipenyu.cn

[Q72] 查看索引
来源：http://wlt.svipenyu.cn

SHOW INDEX FROM users;
来源：http://jko.zhengqikj.top

[Q73] 查看表状态
来源：http://xqz.xuanzx.com

SHOW TABLE STATUS LIKE 'users';
来源：http://bzw.havefunace.top

[Q74] 强制使用索引
来源：http://zde.zycfv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bvh.epnwcf.com

[Q75] 日期格式化
来源：http://biy.ydjk.org.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://trf.zhoulong.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jit.xuanzx.com

[Q76] 按天统计
来源：http://hjy.ehwqpu.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zfw.redwolf501.top

[Q77] 时间加减
来源：http://nca.shanyushiyangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wrq.guannengcc.top

[Q78] 当前时间
来源：http://mpn.xuetiantiany.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kdk.mhx1999.top

[Q79] 字符串拼接
来源：http://fvd.hammf.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jwp.chenjidiqi.icu

[Q80] 字符串截取
来源：http://olm.redwolf501.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cfw.shanyushiyangkeji.top

[Q81] 字符串替换
来源：http://twy.bbcook.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jin.shangyingyoupin.top

[Q82] 字符长度与字节长度
来源：http://ktv.jinyuanbaomall.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gvc.hnqzz.top

[Q83] 大小写转换
来源：http://hrz.yongpay.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oqh.redwolf501.top

[Q84] 去除首尾空格
来源：http://hmi.shanyushiyangkeji.top

SELECT TRIM(name) FROM users;
来源：http://xtm.hesvh.cn

[Q85] 数值取整
来源：http://biz.nwbrower.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://grq.vehdjk.com

[Q86] 读取 JSON 字段
来源：http://ncw.kuanghao11.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ptz.fehbvm.com

[Q87] JSON 字段做条件
来源：http://cdk.uphjek.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hww.sufxvd.cn

[Q88] 行转列（条件聚合）
来源：http://krg.snrcjt.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hgq.nwbrower.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tuw.nanxuanxn.top

[Q89] 判断表是否存在
来源：http://rbl.xziqi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dbt.nanxuanxn.top

[Q90] 生成序号列
来源：http://lqa.ivvv.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yao.yj20258.top

================================================================================
来源：http://sqr.chenjidiqi.icu

R. Bash 专题
来源：http://qwp.jiagoushi.top

================================================================================
来源：http://ycz.hysaishi.cn

[R01] shebang 与严格模式
来源：http://lha.pycfn.com

#!/usr/bin/env bash
来源：http://xcq.hesvh.cn

set -euo pipefail
来源：http://uah.dashuyun.cn

[R02] 变量赋值与使用
来源：http://oyb.sjlbkw.cn

name="Tom"; echo "$name"
来源：http://uwq.jqgfzy.top

[R03] 只读变量
来源：http://mzj.316326.xyz

readonly PI=3.14
来源：http://svt.haohaochexian.top

[R04] 位置参数
来源：http://nmi.guannengcc.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ckg.jqgfzy.top

[R05] 参数默认值
来源：http://xrq.ctjpmb.com

name="${1:-default}"
来源：http://fiu.cdnleiting.top

[R06] 判断命令是否存在
来源：http://trh.yfazqb.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jym.havefunace.top

[R07] if 判断文件
来源：http://hzw.fehbvm.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://paq.gogol.net.cn

[R08] 数值比较
来源：http://jvi.yj20258888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mnj.cheryme.top

[R09] 字符串比较
来源：http://lvj.jlsjyb.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gwk.nanxuanxn.top

[R10] 正则匹配
来源：http://bas.ctjpmb.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gbz.zhijiandao.cn

[R11] case 多分支
来源：http://mxy.fehbvm.com

case "$1" in
来源：http://txa.tian-w.cn

start) echo "启动" ;;
来源：http://qep.yonumen.top

stop)  echo "停止" ;;
来源：http://dop.haohaochexian.top

*)     echo "未知命令" ;;
来源：http://ktn.daxiang520.top

esac
来源：http://vlk.dashuyun.cn

[R12] for 遍历文件
来源：http://wnw.yj202588.top

for f in *.txt; do echo "$f"; done
来源：http://yty.jinqigufen.top

[R13] for 计数循环
来源：http://jjx.haohaochexian.top

for i in {1..10}; do echo "$i"; done
来源：http://pst.hfpthk.cn

[R14] C 风格 for
来源：http://bkm.chenjidiqi.icu

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jdu.nwbrower.top

[R15] while 逐行读文件
来源：http://oib.andypj.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bve.haohaochexian.top

[R16] until 等待条件
来源：http://shg.pengpengdd.cyou

until [[ -f done.flag ]]; do sleep 1; done
来源：http://oqu.jianghu66.top

[R17] 数组定义与取值
来源：http://ddk.zdqjudy.top

arr=(a b c); echo "${arr[0]}"
来源：http://rgn.yj202588.top

[R18] 遍历数组
来源：http://qww.ehwqpu.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cbj.yangfankeji.com

[R19] 数组长度
来源：http://slj.hesvh.cn

echo "${#arr[@]}"
来源：http://pwt.ydzc1.top

[R20] 关联数组（字典）
来源：http://trh.zhoulong.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cxj.ctjpmb.com

[R21] 字符串长度
来源：http://sui.shanyushiyangkeji.top

echo "${#s}"
来源：http://npi.xylfe.cn

[R22] 截取子串
来源：http://iwo.feifeiyinyue.top

echo "${s:0:5}"
来源：http://knh.ydzc1.top

[R23] 字符串替换
来源：http://rsh.guowangkeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pay.jqgfzy.top

[R24] 大小写转换
来源：http://qnk.fengsongda.top

echo "${s^^}"; echo "${s,,}"
来源：http://hgw.fzhhl.top

[R25] 去后缀 / 去前缀
来源：http://hlf.fanxiaobao.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://ufh.gotoacloud.top

[R26] 命令替换
来源：http://kgb.ivvv.top

now=$(date +%F); echo "$now"
来源：http://vbh.zhixingplan.top

[R27] 算术展开
来源：http://vvx.xuetiantiany.cn

echo $((1 + 2 * 3))
来源：http://lir.yangfankeji.com

[R28] 浮点运算
来源：http://sgo.nanxuanxn.top

echo "scale=2; 10/3" | bc
来源：http://mnc.daria6918.cn

[R29] 定义函数
来源：http://zym.sysykeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dhg.hesvh.cn

[R30] 函数返回状态码
来源：http://txr.mhx1999.top

f() { return 0; }; f || echo "失败了"
来源：http://ztc.jinyuanbaomall.cn

[R31] 局部变量
来源：http://inv.yonumen.top

f() { local x=1; echo "$x"; }
来源：http://uen.yj20258888.top

[R32] 参数个数校验
来源：http://kug.daxiang520.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bnc.yuanzhike.top

[R33] 捕获错误并提示行号
来源：http://gdl.zhixingplan.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qpc.ivvv.top

[R34] 退出时清理
来源：http://wbi.9152youxi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zsk.ywan-chungtsiang.top

[R35] 后台执行并等待
来源：http://eqw.zycfv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jjd.52xcode.cn

[R36] 并发执行多个任务
来源：http://jem.jqgfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ydp.fktsv.cn

[R37] 把输出赋给变量
来源：http://dbj.nwbrower.top

files=$(ls -1)
来源：http://qen.yongpay.top

[R38] 管道串联
来源：http://fts.snrcjt.cn

cat a.txt | grep -i error | wc -l
来源：http://pxm.vehdjk.com

[R39] 重定向标准输出与错误
来源：http://kdd.316326.xyz

cmd > out.log 2>&1
来源：http://joj.nanxuanxn.top

[R40] 追加写日志
来源：http://qlo.xuanzx.com

echo "log" >> out.log
来源：http://tyy.zdqjudy.top

[R41] 丢弃输出
来源：http://rso.smart0.xyz

cmd >/dev/null 2>&1
来源：http://bic.jinghuilouyu.cn

[R42] 输入重定向
来源：http://kut.epnwcf.com

wc -l < a.txt
来源：http://zhk.316326.xyz

[R43] 按名字查找文件
来源：http://owk.xylfe.cn

find . -name "*.log" -type f
来源：http://dqn.yongpay.top

[R44] 按修改时间查找
来源：http://vwp.daxiang520.top

find . -mtime -7 -type f
来源：http://cbz.0kj1m.cn

[R45] 批量删除
来源：http://ryg.yongpay.top

find . -name "*.tmp" -delete
来源：http://toh.ydzc1.top

[R46] 递归替换文件内容
来源：http://nvs.zhaomingkeji.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kkj.epnwcf.com

[R47] sed 单行替换
来源：http://hiq.nwbrower.top

sed -i 's/foo/bar/g' a.txt
来源：http://iev.xylfe.cn

[R48] awk 取指定列
来源：http://dpt.zhixingplan.top

awk '{print $1, $3}' a.txt
来源：http://tdi.redwolf501.top

[R49] awk 带条件
来源：http://elh.hcnkem.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cjs.zycfv.cn

[R50] awk 求和
来源：http://pco.dianchejie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qqt.zhiwuduotai.top

[R51] 排序去重取前几
来源：http://wjm.ppjwa.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://oyo.jianghu66.top

[R52] 统计行数
来源：http://xpf.svipenyu.cn

wc -l a.txt
来源：http://alj.xuanzx.com

[R53] 查看文件头与实时尾
来源：http://snv.xylfe.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mua.jqgfzy.top

[R54] 比较两个文件
来源：http://gme.zycfv.cn

diff a.txt b.txt
来源：http://rzq.xylfe.cn

[R55] 压缩与解压
来源：http://zlg.jianghu66.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://brj.andypj.xyz

[R56] 远程拷贝
来源：http://azo.bbcook.cn

scp file user@host:/path/
来源：http://lwp.yonumen.top

[R57] 远程执行命令
来源：http://uzb.ydzc1.top

ssh user@host 'uptime'
来源：http://zgu.yongpay.top

[R58] 下载文件
来源：http://pao.kuanghao11.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ypa.cheryme.top

[R59] 发 POST JSON
来源：http://anx.gotoacloud.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jzt.jianghu66.top

[R60] 只看 HTTP 状态码
来源：http://crr.svipenyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ixf.cheryme.top

[R61] 磁盘占用
来源：http://new.gaohongyu789.top

df -h;  du -sh *
来源：http://vfw.meibo888.top

[R62] 找最占空间的文件
来源：http://auq.daria6918.cn

du -ah . | sort -rh | head -10
来源：http://fvn.wangdashe.top

[R63] 内存与进程
来源：http://fge.vqdsnc.cn

free -h;  ps aux | grep nginx
来源：http://wwa.yangfankeji.com

[R64] 结束进程
来源：http://evl.ydzc1.top

kill -9 $(pgrep -f app.py)
来源：http://kox.fzhhl.top

[R65] 查看端口占用
来源：http://fau.sjlbkw.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ota.jinghuilouyu.cn

[R66] 定时任务
来源：http://rau.daria6918.cn

crontab -e;  crontab -l
来源：http://kpd.ivvv.top

[R67] 生成随机十六进制串
来源：http://yaw.feifeiyinyue.top

openssl rand -hex 16
来源：http://tac.yj20258888.top

[R68] 计算文件校验值
来源：http://rps.cqqwz.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tav.9152youxi.cn

[R69] 生成随机密码
来源：http://ipm.dashuyun.cn

head -c 16 /dev/urandom | base64
来源：http://goe.52xcode.cn

[R70] 时间戳与互转
来源：http://qza.ehwqpu.com

date +%s;  date -d @1700000000
来源：http://mlv.vqdsnc.cn

[R71] 日期格式化
来源：http://znr.jqgufenzy.top


<!-- 参考信息 -->