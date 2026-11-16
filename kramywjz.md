代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qop.zhiwuduotai.top

[Q20] IN 列表
来源：http://cdo.yangfankeji.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://czb.vqdsnc.cn

[Q21] 空值判断
来源：http://hhs.nwbrower.top

SELECT * FROM users WHERE email IS NULL;
来源：http://vww.havefunace.top

[Q22] 排序
来源：http://fjt.hywenlv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fia.wangdashe.top

[Q23] 分页
来源：http://omy.xziqi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://snk.yangfankeji.com

[Q24] 去重
来源：http://ilb.quarkkingdee.top

SELECT DISTINCT city FROM users;
来源：http://ifk.jinqigfzy.top

[Q25] 只取前 N 条
来源：http://toa.haohaochexian.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zwb.yvedp.cn

[Q26] 计数
来源：http://hls.kuanghao11.cn

SELECT COUNT(*) FROM users;
来源：http://ywh.ywan-chungtsiang.top

[Q27] 条件计数
来源：http://vlz.aizwys.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xth.jqgfzy.top

[Q28] 求和与平均
来源：http://pyy.hfpthk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lbr.ydzc1.top

[Q29] 最大最小值
来源：http://tkb.ehwqpu.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://hgx.jinyuanbaomall.cn

[Q30] 分组统计
来源：http://mqq.birdmap.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lcs.fengsongda.top

[Q31] 分组后过滤
来源：http://vch.jlsjyb.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qdn.tianlin.xyz

[Q32] 分组拼接字符串
来源：http://ena.andypj.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eqg.ehwqpu.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uzz.sjlbkw.cn

[Q33] 多列分组
来源：http://btm.gaohongyu789.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qzx.havefunace.top

[Q34] 每组取第一条
来源：http://pdx.feifeiyinyue.top

SELECT * FROM (
来源：http://hpw.xziqi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kfl.tianlin.xyz

) t WHERE rn = 1;
来源：http://wlv.bbcook.cn

[Q35] 内连接
来源：http://srv.sufxvd.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://est.fehbvm.com

[Q36] 左连接
来源：http://eqf.nwbrower.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bgy.mhx1999.top

[Q37] 右连接
来源：http://vvb.jiagoushi.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ben.cheryme.top

[Q38] 全外连接（PostgreSQL）
来源：http://gif.cdnleiting.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wow.316326.xyz

[Q39] 自连接（查上下级）
来源：http://jrn.nanxinkj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://hua.jinqigfzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gjh.hammf.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lzq.vehdjk.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qqt.zhengqikj.top

[Q41] 多表连接
来源：http://aet.jiagoushi.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ylz.hesvh.cn

JOIN users u ON u.id = o.user_id
来源：http://jvp.yangfankeji.com

JOIN products p ON p.id = o.product_id;
来源：http://bil.andypj.xyz

[Q42] 连接条件附加过滤
来源：http://kej.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u
来源：http://kpm.tian-w.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xdt.hfpthk.cn

[Q43] 标量子查询
来源：http://bge.dashuyun.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gzb.quarkkingdee.top

[Q44] IN 子查询
来源：http://mxw.hesvh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xtt.ctjpmb.com

[Q45] EXISTS 判断存在
来源：http://vsa.redwolf501.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zwh.cdnleiting.top

[Q46] NOT EXISTS 判断不存在
来源：http://cvh.jqgufenzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ejc.hfpthk.cn

[Q47] 与平均值比较
来源：http://liu.ctjpmb.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://csd.haohaochexian.top

[Q48] CTE 公用表表达式
来源：http://qyc.yj20258.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ikm.zycfv.cn

SELECT * FROM t WHERE c > 5;
来源：http://vqq.hongshengwenyu.top

[Q49] 更新单行
来源：http://xvg.dashuyun.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gbf.sjlbkw.cn

[Q50] 批量更新
来源：http://kfc.fktsv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xth.tian-w.cn

[Q51] 用子查询更新
来源：http://mge.ybcxt.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zld.daxiang520.top

[Q52] 删除指定行
来源：http://rdb.hywenlv.cn

DELETE FROM users WHERE id = 10;
来源：http://odd.wangdashe.top

[Q53] 按条件删除
来源：http://tpu.zhijiandao.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yjk.sweek.top

[Q54] 清空表
来源：http://xak.chenlongwang.top

TRUNCATE TABLE logs;
来源：http://dka.yanxiufei.cn

[Q55] 排名（并列占位）
来源：http://ogf.hfpthk.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zsz.yongpay.top

[Q56] 密集排名（并列不占位）
来源：http://aid.hammf.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kwz.hnxiangtu.top

[Q57] 行号
来源：http://miv.316326.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pca.smart0.xyz

[Q58] 累计求和
来源：http://ynt.tanke756.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wfv.chenzaomai.com

[Q59] 分组内累计
来源：http://bnr.yj202588.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zqs.gogol.net.cn

[Q60] 取上一行 / 下一行
来源：http://sbx.hnqzz.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kti.zycfv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uwd.jqgufenzy.top

[Q61] 移动平均
来源：http://twb.jiagoushi.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iwv.zdbjq.cn

[Q62] 分组占比
来源：http://dok.kuanghao11.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ngm.dashuyun.cn

[Q63] 开启事务
来源：http://rmt.aibaodan.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://svl.0kj1m.cn

[Q64] 提交事务
来源：http://ovg.cqqwz.cn

COMMIT;
来源：http://hvu.shzxlz.cn

[Q65] 回滚事务
来源：http://jbp.yongpay.top

ROLLBACK;
来源：http://wpb.ydzc1.top

[Q66] 行锁查询
来源：http://tpy.shanyushiyangkeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://umg.meibo888.top

[Q67] 设置隔离级别
来源：http://ras.yuxming.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://iuw.dianchejie.cn

[Q68] 保存点
来源：http://xwy.xylfe.cn

SAVEPOINT sp1;
来源：http://xej.svipenyu.cn

ROLLBACK TO sp1;
来源：http://vmh.yj202588.top

[Q69] 查看执行计划
来源：http://kdu.zhaomingkeji.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vfl.ppjwa.cn

[Q70] 更新统计信息
来源：http://rjn.yueranfly.top

ANALYZE TABLE users;
来源：http://qcs.hnxiangtu.top

[Q71] 查看建表语句
来源：http://ixu.jinghuilouyu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sam.cqqwz.cn

[Q72] 查看索引
来源：http://epo.bjfxy.top

SHOW INDEX FROM users;
来源：http://onw.shzxlz.cn

[Q73] 查看表状态
来源：http://gqw.haohaochexian.top

SHOW TABLE STATUS LIKE 'users';
来源：http://zfz.fehbvm.com

[Q74] 强制使用索引
来源：http://ztl.fengsongda.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://afu.hnqzz.top

[Q75] 日期格式化
来源：http://gry.tanke756.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://soa.quarkkingdee.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yst.aibaodan.cn

[Q76] 按天统计
来源：http://own.jinqigfzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wah.aizwys.cn

[Q77] 时间加减
来源：http://fuh.daria6918.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mtc.tian-w.cn

[Q78] 当前时间
来源：http://zmb.cdnleiting.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rqg.cashguo.top

[Q79] 字符串拼接
来源：http://fio.yanxiufei.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tpa.zhongyouzk.top

[Q80] 字符串截取
来源：http://xpd.hammf.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yzi.ybcxt.top

[Q81] 字符串替换
来源：http://tnn.epnwcf.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xcs.zhiwuduotai.top

[Q82] 字符长度与字节长度
来源：http://zdd.fehbvm.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zvn.guowangkeji.top

[Q83] 大小写转换
来源：http://ciz.gotoacloud.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vzi.fktsv.cn

[Q84] 去除首尾空格
来源：http://zir.fanxiaobao.xyz

SELECT TRIM(name) FROM users;
来源：http://uyg.jianghu66.top

[Q85] 数值取整
来源：http://zvk.hfpthk.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://crr.chenzaomai.com

[Q86] 读取 JSON 字段
来源：http://lga.guowangkeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nqh.bbcook.cn

[Q87] JSON 字段做条件
来源：http://ldf.c1oappe.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jks.shuidangran.top

[Q88] 行转列（条件聚合）
来源：http://qla.jianghu66.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vaw.hnxiangtu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zii.epnwcf.com

[Q89] 判断表是否存在
来源：http://spd.fehbvm.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pvg.zdqjudy.top

[Q90] 生成序号列
来源：http://ane.daria6918.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ssw.tanke756.top

================================================================================
来源：http://mvc.dashuyun.cn

R. Bash 专题
来源：http://fne.tian-w.cn

================================================================================
来源：http://nzn.hnqzz.top

[R01] shebang 与严格模式
来源：http://cff.ppjwa.cn

#!/usr/bin/env bash
来源：http://err.fzhhl.top

set -euo pipefail
来源：http://zzi.shanyushiyangtech.top

[R02] 变量赋值与使用
来源：http://rjn.xinyue.icu

name="Tom"; echo "$name"
来源：http://vcs.jqgfzy.top

[R03] 只读变量
来源：http://bfy.shanyushiyangtech.top

readonly PI=3.14
来源：http://cpo.yonumen.top

[R04] 位置参数
来源：http://tnc.zhongyouzk.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xjs.sjlbkw.cn

[R05] 参数默认值
来源：http://hrv.iojbl.cn

name="${1:-default}"
来源：http://oie.guowangkeji.top

[R06] 判断命令是否存在
来源：http://vqx.feifeiyinyue.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bgu.yj202588.top

[R07] if 判断文件
来源：http://gnc.yangfankeji.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vsl.sufxvd.cn

[R08] 数值比较
来源：http://mux.gogol.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://chl.zdbjq.cn

[R09] 字符串比较
来源：http://cdb.sysykeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sym.jinqigfzy.top

[R10] 正则匹配
来源：http://vfv.chenjidiqi.icu

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vqz.hammf.cn

[R11] case 多分支
来源：http://txn.ehwqpu.com

case "$1" in
来源：http://jdb.cucudq.cn

start) echo "启动" ;;
来源：http://ybx.0kj1m.cn

stop)  echo "停止" ;;
来源：http://opp.chenzaomai.com

*)     echo "未知命令" ;;
来源：http://xgz.feifeiyinyue.top

esac
来源：http://xzz.shzxlz.cn

[R12] for 遍历文件
来源：http://cul.yuxming.cn

for f in *.txt; do echo "$f"; done
来源：http://wbb.zhoulong.xyz

[R13] for 计数循环
来源：http://bar.cqqwz.cn

for i in {1..10}; do echo "$i"; done
来源：http://dev.redwolf501.top

[R14] C 风格 for
来源：http://ugy.nanxinkj.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tqq.yuanzhike.top

[R15] while 逐行读文件
来源：http://nsd.iojbl.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://eak.nanxuanxn.top

[R16] until 等待条件
来源：http://nta.jianghu66.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qiy.ybcxt.top

[R17] 数组定义与取值
来源：http://knp.yueranfly.top

arr=(a b c); echo "${arr[0]}"
来源：http://bsm.ydzc1.top

[R18] 遍历数组
来源：http://cos.yj20258.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://okq.yj20258888.top

[R19] 数组长度
来源：http://tms.jinqigufen.top

echo "${#arr[@]}"
来源：http://sqq.yj202588.top

[R20] 关联数组（字典）
来源：http://zeb.zdbjq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tpt.shanyushiyangtech.top

[R21] 字符串长度
来源：http://poi.jqgufenzy.top

echo "${#s}"
来源：http://hhq.nanxuanxn.top

[R22] 截取子串
来源：http://ybx.mhx1999.top

echo "${s:0:5}"
来源：http://yni.jianghu66.top

[R23] 字符串替换
来源：http://aux.jinqigufen.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wqr.chenlongwang.top

[R24] 大小写转换
来源：http://efo.shanyushiyangtech.top

echo "${s^^}"; echo "${s,,}"
来源：http://gtr.daria6918.cn

[R25] 去后缀 / 去前缀
来源：http://rmm.havefunace.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://fga.svipenyu.cn

[R26] 命令替换
来源：http://nyc.jinyuanbaomall.cn

now=$(date +%F); echo "$now"
来源：http://kse.tianlin.xyz

[R27] 算术展开
来源：http://uhy.jlsjyb.cn

echo $((1 + 2 * 3))
来源：http://agl.fehbvm.com

[R28] 浮点运算
来源：http://wlq.fengsongda.top

echo "scale=2; 10/3" | bc
来源：http://vpa.yueranfly.top

[R29] 定义函数
来源：http://pqv.hammf.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vnm.cucudq.cn

[R30] 函数返回状态码
来源：http://paz.zhoulong.xyz

f() { return 0; }; f || echo "失败了"
来源：http://vkl.chenlongwang.top

[R31] 局部变量
来源：http://xmy.ydzc1.top

f() { local x=1; echo "$x"; }
来源：http://huy.tian-w.cn

[R32] 参数个数校验
来源：http://rjs.yongpay.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tci.hnxiangtu.top

[R33] 捕获错误并提示行号
来源：http://emd.uphjek.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mru.hcnkem.com

[R34] 退出时清理
来源：http://uun.tanke756.top

trap 'rm -f "$tmp"' EXIT
来源：http://ncy.havefunace.top

[R35] 后台执行并等待
来源：http://qtt.jqgfzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://zpx.sweek.top

[R36] 并发执行多个任务
来源：http://gzy.ivvv.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bib.daria6918.cn

[R37] 把输出赋给变量
来源：http://wsi.shanyushiyangtech.top

files=$(ls -1)
来源：http://dmp.gaohongyu789.top

[R38] 管道串联
来源：http://ioi.uphjek.com

cat a.txt | grep -i error | wc -l
来源：http://oja.tianlin.xyz

[R39] 重定向标准输出与错误
来源：http://stx.ywan-chungtsiang.top

cmd > out.log 2>&1
来源：http://wzj.chenlongwang.top

[R40] 追加写日志
来源：http://jsv.jiagoushi.top

echo "log" >> out.log
来源：http://jjx.birdmap.top

[R41] 丢弃输出
来源：http://jkw.chenjidiqi.icu

cmd >/dev/null 2>&1
来源：http://wdc.smart0.xyz

[R42] 输入重定向
来源：http://gtb.jinyuanbaomall.cn

wc -l < a.txt
来源：http://puh.cucudq.cn

[R43] 按名字查找文件
来源：http://eph.ehwqpu.com

find . -name "*.log" -type f
来源：http://aeh.cheryme.top

[R44] 按修改时间查找
来源：http://nrf.yongpay.top

find . -mtime -7 -type f
来源：http://gyo.wangshuangyany.cn

[R45] 批量删除
来源：http://dto.uphjek.com

find . -name "*.tmp" -delete
来源：http://pnp.dianchejie.cn

[R46] 递归替换文件内容
来源：http://ytr.pengpengdd.cyou

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wuz.shangyingyoupin.top

[R47] sed 单行替换
来源：http://wyh.ivvv.top

sed -i 's/foo/bar/g' a.txt
来源：http://mqf.daxiang520.top

[R48] awk 取指定列
来源：http://vxc.fanxiaobao.xyz

awk '{print $1, $3}' a.txt
来源：http://dwm.jinghuilouyu.cn

[R49] awk 带条件
来源：http://ijd.jinqigufen.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ymo.aibaodan.cn

[R50] awk 求和
来源：http://ffd.cqqwz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nnq.aibaodan.cn

[R51] 排序去重取前几
来源：http://mqh.pycfn.com

sort a.txt | uniq -c | sort -rn | head
来源：http://ari.tianlin.xyz

[R52] 统计行数
来源：http://afu.zhongyouzk.top

wc -l a.txt
来源：http://yfk.yongpay.top

[R53] 查看文件头与实时尾
来源：http://eug.jinyuanbaomall.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qht.sweek.top

[R54] 比较两个文件
来源：http://kkd.yvedp.cn

diff a.txt b.txt
来源：http://qsg.hammf.cn

[R55] 压缩与解压
来源：http://qrv.xuanzx.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mjf.quarkkingdee.top

[R56] 远程拷贝
来源：http://xup.hysaishi.cn

scp file user@host:/path/
来源：http://mao.yuxming.cn

[R57] 远程执行命令
来源：http://ign.tian-w.cn

ssh user@host 'uptime'
来源：http://cfe.sufxvd.cn

[R58] 下载文件
来源：http://wtq.cucudq.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jzg.andypj.xyz

[R59] 发 POST JSON
来源：http://kui.0kj1m.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://olh.zycfv.cn

[R60] 只看 HTTP 状态码
来源：http://rpv.kuanghao11.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wts.pycfn.com

[R61] 磁盘占用
来源：http://lkl.zycfv.cn

df -h;  du -sh *
来源：http://slw.daxiang520.top

[R62] 找最占空间的文件
来源：http://jvf.52xcode.cn

du -ah . | sort -rh | head -10
来源：http://gtu.yuxming.cn

[R63] 内存与进程
来源：http://rbo.hfpthk.cn

free -h;  ps aux | grep nginx
来源：http://vcy.meibo888.top

[R64] 结束进程
来源：http://kab.yueranfly.top

kill -9 $(pgrep -f app.py)
来源：http://pmj.zhongyouzk.top

[R65] 查看端口占用
来源：http://pwl.havefunace.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lnh.wangshuangyany.cn

[R66] 定时任务
来源：http://kne.fanxiaobao.xyz

crontab -e;  crontab -l
来源：http://sdw.yfazqb.com

[R67] 生成随机十六进制串
来源：http://ean.yangfankeji.com

openssl rand -hex 16
来源：http://xin.ydzc1.top

[R68] 计算文件校验值
来源：http://epv.fehbvm.com

sha256sum a.txt;  md5sum a.txt
来源：http://afb.jinghuilouyu.cn

[R69] 生成随机密码
来源：http://vce.quarkkingdee.top


<!-- 参考信息 -->