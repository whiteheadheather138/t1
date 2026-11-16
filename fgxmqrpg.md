代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://veu.9152youxi.cn

[Q24] 去重
来源：http://lzw.jqgufenzy.top

SELECT DISTINCT city FROM users;
来源：http://amj.wangdashe.top

[Q25] 只取前 N 条
来源：http://aky.sxryk.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qzf.fehbvm.com

[Q26] 计数
来源：http://ghv.yj20258888.top

SELECT COUNT(*) FROM users;
来源：http://nlf.zdbjq.cn

[Q27] 条件计数
来源：http://rhl.uphjek.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yqw.jinqigfzy.top

[Q28] 求和与平均
来源：http://xds.birdmap.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lxl.smart0.xyz

[Q29] 最大最小值
来源：http://cby.birdmap.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://lhu.tianlin.xyz

[Q30] 分组统计
来源：http://shh.fengsongda.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uaa.zdbjq.cn

[Q31] 分组后过滤
来源：http://bqw.zycfv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://etr.xuanzx.com

[Q32] 分组拼接字符串
来源：http://fcf.xylfe.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zkx.sufxvd.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dkl.jiagoushi.top

[Q33] 多列分组
来源：http://rgk.shuidangran.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ihe.hammf.cn

[Q34] 每组取第一条
来源：http://ekm.xziqi.cn

SELECT * FROM (
来源：http://nba.zhengqikj.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jky.quarkkingdee.top

) t WHERE rn = 1;
来源：http://fcn.zdqjudy.top

[Q35] 内连接
来源：http://qiz.xuetiantiany.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://apy.hfpthk.cn

[Q36] 左连接
来源：http://sww.daria6918.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fhq.zhixingplan.top

[Q37] 右连接
来源：http://dks.haohaochexian.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rla.hnxiangtu.top

[Q38] 全外连接（PostgreSQL）
来源：http://iua.yvedp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://stv.tian-w.cn

[Q39] 自连接（查上下级）
来源：http://kvi.yongpay.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://cht.yfazqb.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oua.hysaishi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://apt.cucudq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://emp.zhiwuduotai.top

[Q41] 多表连接
来源：http://qsp.gotoacloud.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://gka.redwolf501.top

JOIN users u ON u.id = o.user_id
来源：http://mpn.cdnleiting.top

JOIN products p ON p.id = o.product_id;
来源：http://tqf.birdmap.top

[Q42] 连接条件附加过滤
来源：http://vdg.pengpengdd.cyou

SELECT u.name, o.amount FROM users u
来源：http://kjk.pengpengdd.cyou

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wie.ybcxt.top

[Q43] 标量子查询
来源：http://wlj.xuetiantiany.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nui.smart0.xyz

[Q44] IN 子查询
来源：http://ytv.52xcode.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qpm.52xcode.cn

[Q45] EXISTS 判断存在
来源：http://hkd.yfazqb.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://exy.shangyingyoupin.top

[Q46] NOT EXISTS 判断不存在
来源：http://fil.haohaochexian.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ttg.cucudq.cn

[Q47] 与平均值比较
来源：http://sbh.jqgufenzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rce.vehdjk.com

[Q48] CTE 公用表表达式
来源：http://loa.nwbrower.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vva.yangfankeji.com

SELECT * FROM t WHERE c > 5;
来源：http://mjf.chenjidiqi.icu

[Q49] 更新单行
来源：http://uuh.zhongyouzk.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://occ.vqdsnc.cn

[Q50] 批量更新
来源：http://rgv.xuanzx.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kpz.dianchejie.cn

[Q51] 用子查询更新
来源：http://kwf.52xcode.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pbz.sxryk.cn

[Q52] 删除指定行
来源：http://utj.ydzc1.top

DELETE FROM users WHERE id = 10;
来源：http://gww.hongshengwenyu.top

[Q53] 按条件删除
来源：http://bpc.zdqjudy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://iyx.hysaishi.cn

[Q54] 清空表
来源：http://vfa.wangdashe.top

TRUNCATE TABLE logs;
来源：http://jzr.xylfe.cn

[Q55] 排名（并列占位）
来源：http://vos.vqdsnc.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pjn.hnqzz.top

[Q56] 密集排名（并列不占位）
来源：http://qxr.gotoacloud.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rhi.hfpthk.cn

[Q57] 行号
来源：http://fdv.vehdjk.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kpi.meibo888.top

[Q58] 累计求和
来源：http://lqp.yangfankeji.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nsm.hongshengwenyu.top

[Q59] 分组内累计
来源：http://fuh.yuanzhike.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kuo.9152youxi.cn

[Q60] 取上一行 / 下一行
来源：http://yfv.epnwcf.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://foa.fengsongda.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cyv.gotoacloud.top

[Q61] 移动平均
来源：http://uny.ctjpmb.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uzg.shangyingyoupin.top

[Q62] 分组占比
来源：http://kqy.bjfxy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://iho.yueranfly.top

[Q63] 开启事务
来源：http://ohr.nanxinkj.top

START TRANSACTION;                -- 或 BEGIN
来源：http://aqr.52xcode.cn

[Q64] 提交事务
来源：http://cjf.kuanghao11.cn

COMMIT;
来源：http://vtr.chenzaomai.com

[Q65] 回滚事务
来源：http://rvx.yj20258888.top

ROLLBACK;
来源：http://dio.pycfn.com

[Q66] 行锁查询
来源：http://utj.jinqigfzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jlb.yongpay.top

[Q67] 设置隔离级别
来源：http://zqz.fanxiaobao.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gav.cqqwz.cn

[Q68] 保存点
来源：http://ydk.bjfxy.top

SAVEPOINT sp1;
来源：http://afd.pengpengdd.cyou

ROLLBACK TO sp1;
来源：http://gxm.sxryk.cn

[Q69] 查看执行计划
来源：http://gth.gotoacloud.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lsh.feifeiyinyue.top

[Q70] 更新统计信息
来源：http://vxr.fzhhl.top

ANALYZE TABLE users;
来源：http://dje.yanxiufei.cn

[Q71] 查看建表语句
来源：http://rmj.jqgfzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cxz.birdmap.top

[Q72] 查看索引
来源：http://plq.fehbvm.com

SHOW INDEX FROM users;
来源：http://wqb.bbcook.cn

[Q73] 查看表状态
来源：http://blu.fanxiaobao.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://wtd.jinqigfzy.top

[Q74] 强制使用索引
来源：http://ago.redwolf501.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ukp.shangyingyoupin.top

[Q75] 日期格式化
来源：http://edg.guowangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://spe.gogol.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ptx.gogol.net.cn

[Q76] 按天统计
来源：http://jri.zycfv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://aqc.52xcode.cn

[Q77] 时间加减
来源：http://eoy.jinyuanbaomall.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wwb.cashguo.top

[Q78] 当前时间
来源：http://pin.chenzaomai.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ltr.uphjek.com

[Q79] 字符串拼接
来源：http://asd.aibaodan.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://flb.gogol.net.cn

[Q80] 字符串截取
来源：http://znj.gogol.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dhp.0kj1m.cn

[Q81] 字符串替换
来源：http://qpo.zhixingplan.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qbx.iojbl.cn

[Q82] 字符长度与字节长度
来源：http://auc.uphjek.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gji.hnxiangtu.top

[Q83] 大小写转换
来源：http://blj.shanyushiyangkeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ltf.ctjpmb.com

[Q84] 去除首尾空格
来源：http://hha.yanxiufei.cn

SELECT TRIM(name) FROM users;
来源：http://euc.xingfuxueyuan.xyz

[Q85] 数值取整
来源：http://qhq.gzhubu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gxi.birdmap.top

[Q86] 读取 JSON 字段
来源：http://odb.shangyingyoupin.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uwd.feifeiyinyue.top

[Q87] JSON 字段做条件
来源：http://ras.jqgfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gjd.zycfv.cn

[Q88] 行转列（条件聚合）
来源：http://zzc.andypj.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cif.havefunace.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://not.52xcode.cn

[Q89] 判断表是否存在
来源：http://zej.jinyuanbaomall.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wtc.jlsjyb.cn

[Q90] 生成序号列
来源：http://agh.zycfv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nhz.sjlbkw.cn

================================================================================
来源：http://aox.tian-w.cn

R. Bash 专题
来源：http://lix.wangshuangyany.cn

================================================================================
来源：http://qxy.snrcjt.cn

[R01] shebang 与严格模式
来源：http://wkk.shzxlz.cn

#!/usr/bin/env bash
来源：http://dsk.uphjek.com

set -euo pipefail
来源：http://sff.9152youxi.cn

[R02] 变量赋值与使用
来源：http://nmr.sweek.top

name="Tom"; echo "$name"
来源：http://tru.wangdashe.top

[R03] 只读变量
来源：http://kbb.ppjwa.cn

readonly PI=3.14
来源：http://fiq.shanyushiyangtech.top

[R04] 位置参数
来源：http://rby.meibo888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qtd.bjfxy.top

[R05] 参数默认值
来源：http://bcp.zhaomingkeji.xyz

name="${1:-default}"
来源：http://kix.hongshengwenyu.top

[R06] 判断命令是否存在
来源：http://qho.mhx1999.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kgo.fehbvm.com

[R07] if 判断文件
来源：http://vwt.dianchejie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uhp.jyoumei.cn

[R08] 数值比较
来源：http://nwq.fehbvm.com

if (( a > b )); then echo "a 更大"; fi
来源：http://srw.quarkkingdee.top

[R09] 字符串比较
来源：http://ebc.quarkkingdee.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pxd.yj20258888.top

[R10] 正则匹配
来源：http://fif.dashuyun.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vca.jlsjyb.cn

[R11] case 多分支
来源：http://pbg.daxiang520.top

case "$1" in
来源：http://sth.xuanzx.com

start) echo "启动" ;;
来源：http://anj.hywenlv.cn

stop)  echo "停止" ;;
来源：http://yuh.sweek.top

*)     echo "未知命令" ;;
来源：http://sdn.chenjidiqi.icu

esac
来源：http://coi.cashguo.top

[R12] for 遍历文件
来源：http://hgo.zhijiandao.cn

for f in *.txt; do echo "$f"; done
来源：http://yqv.zhaomingkeji.xyz

[R13] for 计数循环
来源：http://stx.yanxiufei.cn

for i in {1..10}; do echo "$i"; done
来源：http://uth.zhiwuduotai.top

[R14] C 风格 for
来源：http://tbn.hfpthk.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://peb.ywan-chungtsiang.top

[R15] while 逐行读文件
来源：http://kwy.sysykeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lsy.0kj1m.cn

[R16] until 等待条件
来源：http://dal.ctjpmb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://elk.quarkkingdee.top

[R17] 数组定义与取值
来源：http://ieu.meibo888.top

arr=(a b c); echo "${arr[0]}"
来源：http://acv.iojbl.cn

[R18] 遍历数组
来源：http://zji.zhoulong.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://eak.gaohongyu789.top

[R19] 数组长度
来源：http://flk.zhixingplan.top

echo "${#arr[@]}"
来源：http://rkw.wangdashe.top

[R20] 关联数组（字典）
来源：http://oji.pycfn.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://unz.hesvh.cn

[R21] 字符串长度
来源：http://rer.zdqjudy.top

echo "${#s}"
来源：http://qgw.hywenlv.cn

[R22] 截取子串
来源：http://cps.sweek.top

echo "${s:0:5}"
来源：http://nlm.316326.xyz

[R23] 字符串替换
来源：http://pyh.jinqigufen.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wxc.ydzc1.top

[R24] 大小写转换
来源：http://azg.jiagoushi.top

echo "${s^^}"; echo "${s,,}"
来源：http://iiz.dianchejie.cn

[R25] 去后缀 / 去前缀
来源：http://okz.snrcjt.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fom.andypj.xyz

[R26] 命令替换
来源：http://zmo.shzxlz.cn

now=$(date +%F); echo "$now"
来源：http://utj.316326.xyz

[R27] 算术展开
来源：http://rvi.dashuyun.cn

echo $((1 + 2 * 3))
来源：http://ssm.quarkkingdee.top

[R28] 浮点运算
来源：http://gkg.hywenlv.cn

echo "scale=2; 10/3" | bc
来源：http://wpa.9152youxi.cn

[R29] 定义函数
来源：http://ito.sxryk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://twd.ydzc1.top

[R30] 函数返回状态码
来源：http://ikq.cqqwz.cn

f() { return 0; }; f || echo "失败了"
来源：http://dqx.jqgufenzy.top

[R31] 局部变量
来源：http://daz.ybcxt.top

f() { local x=1; echo "$x"; }
来源：http://bwk.yvedp.cn

[R32] 参数个数校验
来源：http://gce.chenjidiqi.icu

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://amr.hfpthk.cn

[R33] 捕获错误并提示行号
来源：http://lwa.yangfankeji.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ivb.zhixingplan.top

[R34] 退出时清理
来源：http://qpt.hfpthk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vaz.nanxuanxn.top

[R35] 后台执行并等待
来源：http://eyx.xuanzx.com

sleep 5 & pid=$!; wait "$pid"
来源：http://zme.havefunace.top

[R36] 并发执行多个任务
来源：http://crj.fktsv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://orw.jqgfzy.top

[R37] 把输出赋给变量
来源：http://aki.gotoacloud.top

files=$(ls -1)
来源：http://vqy.zdbjq.cn

[R38] 管道串联
来源：http://lbp.gotoacloud.top

cat a.txt | grep -i error | wc -l
来源：http://zgx.zhongyouzk.top

[R39] 重定向标准输出与错误
来源：http://duq.smart0.xyz

cmd > out.log 2>&1
来源：http://cwo.bbcook.cn

[R40] 追加写日志
来源：http://ysr.xuetiantiany.cn

echo "log" >> out.log
来源：http://gjd.yuanzhike.top

[R41] 丢弃输出
来源：http://zsq.316326.xyz

cmd >/dev/null 2>&1
来源：http://zfu.tian-w.cn

[R42] 输入重定向
来源：http://pqw.jqgfzy.top

wc -l < a.txt
来源：http://jxh.shzxlz.cn

[R43] 按名字查找文件
来源：http://fkf.cashguo.top

find . -name "*.log" -type f
来源：http://icv.zhaomingkeji.xyz

[R44] 按修改时间查找
来源：http://fve.nanxinkj.top

find . -mtime -7 -type f
来源：http://ybh.316326.xyz

[R45] 批量删除
来源：http://sqa.c1oappe.top

find . -name "*.tmp" -delete
来源：http://rnr.ydjk.org.cn

[R46] 递归替换文件内容
来源：http://wsf.hammf.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nqq.tian-w.cn

[R47] sed 单行替换
来源：http://kgd.yueranfly.top

sed -i 's/foo/bar/g' a.txt
来源：http://xvs.ydjk.org.cn

[R48] awk 取指定列
来源：http://ure.quarkkingdee.top

awk '{print $1, $3}' a.txt
来源：http://enw.mhx1999.top

[R49] awk 带条件
来源：http://iiz.chenjidiqi.icu

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mwx.hnxiangtu.top

[R50] awk 求和
来源：http://iso.chenzaomai.com

awk '{s += $2} END {print s}' a.txt
来源：http://qkj.sjlbkw.cn

[R51] 排序去重取前几
来源：http://rmy.nanxuanxn.top

sort a.txt | uniq -c | sort -rn | head
来源：http://rtj.birdmap.top

[R52] 统计行数
来源：http://slf.9152youxi.cn

wc -l a.txt
来源：http://efw.xziqi.cn

[R53] 查看文件头与实时尾
来源：http://ncb.zhengqikj.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fcs.aizwys.cn

[R54] 比较两个文件
来源：http://qkl.yueranfly.top

diff a.txt b.txt
来源：http://atg.shzxlz.cn

[R55] 压缩与解压
来源：http://mgs.jinqigfzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://drk.c1oappe.top

[R56] 远程拷贝
来源：http://hdl.bbcook.cn

scp file user@host:/path/
来源：http://cfd.fktsv.cn

[R57] 远程执行命令
来源：http://mam.zhaomingkeji.xyz

ssh user@host 'uptime'
来源：http://cua.fengsongda.top

[R58] 下载文件
来源：http://jde.hnxiangtu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://arq.chenzaomai.com

[R59] 发 POST JSON
来源：http://ihh.jinqigfzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://unq.daxiang520.top

[R60] 只看 HTTP 状态码
来源：http://ghd.hongshengwenyu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rnw.xuetiantiany.cn

[R61] 磁盘占用
来源：http://ppq.birdmap.top

df -h;  du -sh *
来源：http://doq.zhiwuduotai.top

[R62] 找最占空间的文件
来源：http://ivv.bbcook.cn

du -ah . | sort -rh | head -10
来源：http://onc.daria6918.cn

[R63] 内存与进程
来源：http://zph.ivvv.top

free -h;  ps aux | grep nginx
来源：http://pwh.epnwcf.com

[R64] 结束进程
来源：http://mog.zhijiandao.cn

kill -9 $(pgrep -f app.py)
来源：http://bkp.wangdashe.top

[R65] 查看端口占用
来源：http://vsf.zhaomingkeji.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ghg.chenzaomai.com

[R66] 定时任务
来源：http://vxu.smart0.xyz

crontab -e;  crontab -l
来源：http://dmt.yvedp.cn

[R67] 生成随机十六进制串
来源：http://oal.jqgfzy.top

openssl rand -hex 16
来源：http://dmd.pycfn.com

[R68] 计算文件校验值
来源：http://gzu.jqgufenzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://pfo.fzhhl.top

[R69] 生成随机密码
来源：http://flb.hongshengwenyu.top

head -c 16 /dev/urandom | base64
来源：http://ysy.sysykeji.top

[R70] 时间戳与互转
来源：http://vqy.sweek.top

date +%s;  date -d @1700000000
来源：http://qaj.svipenyu.cn

[R71] 日期格式化
来源：http://wme.svipenyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ebz.c1oappe.top

[R72] 等待端口就绪
来源：http://zrm.jinqigufen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://abf.sweek.top

[R73] 分割大日志
来源：http://itu.jinghuilouyu.cn


<!-- 参考信息 -->