代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ene.yanxiufei.cn

[Q26] 计数
来源：http://plq.meibo888.top

SELECT COUNT(*) FROM users;
来源：http://plw.yvedp.cn

[Q27] 条件计数
来源：http://xyc.nanxuanxn.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wxr.chenlongwang.top

[Q28] 求和与平均
来源：http://ruu.hammf.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tlt.316326.xyz

[Q29] 最大最小值
来源：http://tyq.yangfankeji.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://ppm.hesvh.cn

[Q30] 分组统计
来源：http://ebd.shanyushiyangtech.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pdw.ywan-chungtsiang.top

[Q31] 分组后过滤
来源：http://gto.zhoulong.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nlw.yj20258888.top

[Q32] 分组拼接字符串
来源：http://cpk.xziqi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ubf.bbcook.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vrc.gotoacloud.top

[Q33] 多列分组
来源：http://fgo.xylfe.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ajj.hfpthk.cn

[Q34] 每组取第一条
来源：http://vgx.hammf.cn

SELECT * FROM (
来源：http://emt.zycfv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://omk.zdbjq.cn

) t WHERE rn = 1;
来源：http://uhq.xylfe.cn

[Q35] 内连接
来源：http://ekv.ydzc1.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hxs.chenzaomai.com

[Q36] 左连接
来源：http://oxw.dashuyun.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://omw.jinqigufen.top

[Q37] 右连接
来源：http://evu.xuanzx.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zlg.jinyuanbaomall.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ppx.sysykeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://noj.wangdashe.top

[Q39] 自连接（查上下级）
来源：http://epn.zdqjudy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://vlj.zhengqikj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lfw.hysaishi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zya.ppjwa.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pry.yfazqb.com

[Q41] 多表连接
来源：http://xeb.gaohongyu789.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://qnu.yuxming.cn

JOIN users u ON u.id = o.user_id
来源：http://geh.fanxiaobao.xyz

JOIN products p ON p.id = o.product_id;
来源：http://esk.wangshuangyany.cn

[Q42] 连接条件附加过滤
来源：http://gcd.aizwys.cn

SELECT u.name, o.amount FROM users u
来源：http://sxd.jqgfzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xhz.wangshuangyany.cn

[Q43] 标量子查询
来源：http://cgk.yj202588.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qku.epnwcf.com

[Q44] IN 子查询
来源：http://lul.aibaodan.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zrj.fehbvm.com

[Q45] EXISTS 判断存在
来源：http://kre.jyoumei.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wrg.jinghuilouyu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://noi.xuetiantiany.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lkd.aibaodan.cn

[Q47] 与平均值比较
来源：http://jrl.yj20258888.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://aew.yfazqb.com

[Q48] CTE 公用表表达式
来源：http://pap.chenjidiqi.icu

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gci.shanyushiyangtech.top

SELECT * FROM t WHERE c > 5;
来源：http://mbg.shanyushiyangtech.top

[Q49] 更新单行
来源：http://cvl.ppjwa.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kpp.shanyushiyangtech.top

[Q50] 批量更新
来源：http://yqe.ydjk.org.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://asr.jinqigfzy.top

[Q51] 用子查询更新
来源：http://bib.pycfn.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dje.uphjek.com

[Q52] 删除指定行
来源：http://get.jqgufenzy.top

DELETE FROM users WHERE id = 10;
来源：http://ozr.fktsv.cn

[Q53] 按条件删除
来源：http://nsi.hnxiangtu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yhr.svipenyu.cn

[Q54] 清空表
来源：http://ngq.vqdsnc.cn

TRUNCATE TABLE logs;
来源：http://eew.shzxlz.cn

[Q55] 排名（并列占位）
来源：http://cfx.0kj1m.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nbo.bbcook.cn

[Q56] 密集排名（并列不占位）
来源：http://zmn.gaohongyu789.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rqp.bjfxy.top

[Q57] 行号
来源：http://xno.hfpthk.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yfq.sjlbkw.cn

[Q58] 累计求和
来源：http://lnk.zhaomingkeji.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nrp.hnxiangtu.top

[Q59] 分组内累计
来源：http://dzr.hfpthk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gpn.xuetiantiany.cn

[Q60] 取上一行 / 下一行
来源：http://rfh.jqgfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://evk.wangshuangyany.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ank.havefunace.top

[Q61] 移动平均
来源：http://lnb.iojbl.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bak.tanke756.top

[Q62] 分组占比
来源：http://xmk.jinghuilouyu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qtw.hammf.cn

[Q63] 开启事务
来源：http://guh.c1oappe.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gdu.ydzc1.top

[Q64] 提交事务
来源：http://gwo.tian-w.cn

COMMIT;
来源：http://uuj.wangshuangyany.cn

[Q65] 回滚事务
来源：http://iwi.ywan-chungtsiang.top

ROLLBACK;
来源：http://jqj.xinyue.icu

[Q66] 行锁查询
来源：http://esj.ctjpmb.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zsp.haohaochexian.top

[Q67] 设置隔离级别
来源：http://wvy.yfazqb.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zpt.daria6918.cn

[Q68] 保存点
来源：http://xvn.redwolf501.top

SAVEPOINT sp1;
来源：http://byx.cucudq.cn

ROLLBACK TO sp1;
来源：http://lvz.jlsjyb.cn

[Q69] 查看执行计划
来源：http://llw.52xcode.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tuh.wangdashe.top

[Q70] 更新统计信息
来源：http://ett.sweek.top

ANALYZE TABLE users;
来源：http://vgl.birdmap.top

[Q71] 查看建表语句
来源：http://icq.aizwys.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rhb.chenlongwang.top

[Q72] 查看索引
来源：http://gdq.zhaomingkeji.xyz

SHOW INDEX FROM users;
来源：http://muh.cashguo.top

[Q73] 查看表状态
来源：http://iou.meibo888.top

SHOW TABLE STATUS LIKE 'users';
来源：http://nlv.iojbl.cn

[Q74] 强制使用索引
来源：http://tkj.snrcjt.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qxk.xuanzx.com

[Q75] 日期格式化
来源：http://krj.hfpthk.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tfk.zycfv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wel.zhiwuduotai.top

[Q76] 按天统计
来源：http://lxb.jinyuanbaomall.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hqt.svipenyu.cn

[Q77] 时间加减
来源：http://mld.zhiwuduotai.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mad.cheryme.top

[Q78] 当前时间
来源：http://efx.guannengcc.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jtc.pengpengdd.cyou

[Q79] 字符串拼接
来源：http://ndp.shzxlz.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lin.zhoulong.xyz

[Q80] 字符串截取
来源：http://kju.hammf.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oaq.hywenlv.cn

[Q81] 字符串替换
来源：http://fkf.bbcook.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qdj.zhiwuduotai.top

[Q82] 字符长度与字节长度
来源：http://bch.pengpengdd.cyou

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pvd.zhiwuduotai.top

[Q83] 大小写转换
来源：http://zdj.yj202588.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ole.hywenlv.cn

[Q84] 去除首尾空格
来源：http://olx.yangfankeji.com

SELECT TRIM(name) FROM users;
来源：http://pkd.snrcjt.cn

[Q85] 数值取整
来源：http://fjr.svipenyu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://les.yueranfly.top

[Q86] 读取 JSON 字段
来源：http://rjs.ydjk.org.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rfz.kuanghao11.cn

[Q87] JSON 字段做条件
来源：http://dvg.tanke756.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mwj.tarul.cn

[Q88] 行转列（条件聚合）
来源：http://ifh.shzxlz.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sob.yvedp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qus.tarul.cn

[Q89] 判断表是否存在
来源：http://ccw.smart0.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mcq.redwolf501.top

[Q90] 生成序号列
来源：http://txa.xuetiantiany.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://iiu.yuanzhike.top

================================================================================
来源：http://qcq.hcnkem.com

R. Bash 专题
来源：http://bms.cucudq.cn

================================================================================
来源：http://gsq.hesvh.cn

[R01] shebang 与严格模式
来源：http://aam.guannengcc.top

#!/usr/bin/env bash
来源：http://nah.zhixingplan.top

set -euo pipefail
来源：http://zfi.jinyuanbaomall.cn

[R02] 变量赋值与使用
来源：http://zoo.shangyingyoupin.top

name="Tom"; echo "$name"
来源：http://cks.snrcjt.cn

[R03] 只读变量
来源：http://oqf.jianghu66.top

readonly PI=3.14
来源：http://nic.jyoumei.cn

[R04] 位置参数
来源：http://lwp.chenlongwang.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://buv.tianlin.xyz

[R05] 参数默认值
来源：http://rtn.zhengqikj.top

name="${1:-default}"
来源：http://inh.shangyingyoupin.top

[R06] 判断命令是否存在
来源：http://ufm.epnwcf.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hlu.tianlin.xyz

[R07] if 判断文件
来源：http://jgd.fanxiaobao.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lwe.jiagoushi.top

[R08] 数值比较
来源：http://vvc.ppjwa.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://imo.yongpay.top

[R09] 字符串比较
来源：http://ltf.ivvv.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://smi.52xcode.cn

[R10] 正则匹配
来源：http://vzd.ydjk.org.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tby.hysaishi.cn

[R11] case 多分支
来源：http://unf.yuxming.cn

case "$1" in
来源：http://axc.bjfxy.top

start) echo "启动" ;;
来源：http://hro.gotoacloud.top

stop)  echo "停止" ;;
来源：http://hvc.yongpay.top

*)     echo "未知命令" ;;
来源：http://pxp.daxiang520.top

esac
来源：http://vhd.ctjpmb.com

[R12] for 遍历文件
来源：http://ioh.xylfe.cn

for f in *.txt; do echo "$f"; done
来源：http://jvb.jqgufenzy.top

[R13] for 计数循环
来源：http://mgp.ydzc1.top

for i in {1..10}; do echo "$i"; done
来源：http://tmk.chenzaomai.com

[R14] C 风格 for
来源：http://hiz.yanxiufei.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yqj.zdbjq.cn

[R15] while 逐行读文件
来源：http://fmf.chenjidiqi.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hpl.daxiang520.top

[R16] until 等待条件
来源：http://ivl.yfazqb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mfx.tian-w.cn

[R17] 数组定义与取值
来源：http://nvo.shanyushiyangtech.top

arr=(a b c); echo "${arr[0]}"
来源：http://tkk.vehdjk.com

[R18] 遍历数组
来源：http://drp.xylfe.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://txr.shuidangran.top

[R19] 数组长度
来源：http://kyj.jqgfzy.top

echo "${#arr[@]}"
来源：http://qxz.cheryme.top

[R20] 关联数组（字典）
来源：http://pcv.cashguo.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://twf.shanyushiyangkeji.top

[R21] 字符串长度
来源：http://lyc.svipenyu.cn

echo "${#s}"
来源：http://ngg.ppjwa.cn

[R22] 截取子串
来源：http://prt.ywan-chungtsiang.top

echo "${s:0:5}"
来源：http://pzh.fanxiaobao.xyz

[R23] 字符串替换
来源：http://ejo.tanke756.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dgw.epnwcf.com

[R24] 大小写转换
来源：http://zjn.shzxlz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gej.havefunace.top

[R25] 去后缀 / 去前缀
来源：http://ahd.zhengqikj.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://rcd.kuanghao11.cn

[R26] 命令替换
来源：http://brq.hesvh.cn

now=$(date +%F); echo "$now"
来源：http://rzp.ydjk.org.cn

[R27] 算术展开
来源：http://usc.shzxlz.cn

echo $((1 + 2 * 3))
来源：http://rtp.jinqigufen.top

[R28] 浮点运算
来源：http://oxi.cdnleiting.top

echo "scale=2; 10/3" | bc
来源：http://oyk.ydjk.org.cn

[R29] 定义函数
来源：http://gfb.sjlbkw.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://feg.zhiwuduotai.top

[R30] 函数返回状态码
来源：http://tuk.gogol.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://msq.zhixingplan.top

[R31] 局部变量
来源：http://per.hcnkem.com

f() { local x=1; echo "$x"; }
来源：http://ben.shanyushiyangtech.top

[R32] 参数个数校验
来源：http://ayg.quarkkingdee.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cpa.yongpay.top

[R33] 捕获错误并提示行号
来源：http://dua.zhiwuduotai.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bqm.andypj.xyz

[R34] 退出时清理
来源：http://vxc.chenzaomai.com

trap 'rm -f "$tmp"' EXIT
来源：http://kue.iojbl.cn

[R35] 后台执行并等待
来源：http://gub.yuxming.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lvm.yfazqb.com

[R36] 并发执行多个任务
来源：http://ksy.quarkkingdee.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dku.hfpthk.cn

[R37] 把输出赋给变量
来源：http://wji.iojbl.cn

files=$(ls -1)
来源：http://afq.tanke756.top

[R38] 管道串联
来源：http://skp.chenjidiqi.icu

cat a.txt | grep -i error | wc -l
来源：http://ldl.yvedp.cn

[R39] 重定向标准输出与错误
来源：http://ced.haohaochexian.top

cmd > out.log 2>&1
来源：http://msi.tarul.cn

[R40] 追加写日志
来源：http://haf.shanyushiyangtech.top

echo "log" >> out.log
来源：http://zbx.zhijiandao.cn

[R41] 丢弃输出
来源：http://lly.hysaishi.cn

cmd >/dev/null 2>&1
来源：http://ftf.ivvv.top

[R42] 输入重定向
来源：http://xaf.yanxiufei.cn

wc -l < a.txt
来源：http://qhm.vqdsnc.cn

[R43] 按名字查找文件
来源：http://ktg.yvedp.cn

find . -name "*.log" -type f
来源：http://ktq.cheryme.top

[R44] 按修改时间查找
来源：http://wmx.fzhhl.top

find . -mtime -7 -type f
来源：http://bii.redwolf501.top

[R45] 批量删除
来源：http://msv.yangfankeji.com

find . -name "*.tmp" -delete
来源：http://bxp.hongshengwenyu.top

[R46] 递归替换文件内容
来源：http://ytm.epnwcf.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fuj.gotoacloud.top

[R47] sed 单行替换
来源：http://ywi.gzhubu.top

sed -i 's/foo/bar/g' a.txt
来源：http://lqx.fzhhl.top

[R48] awk 取指定列
来源：http://vev.ehwqpu.com

awk '{print $1, $3}' a.txt
来源：http://cxz.9152youxi.cn

[R49] awk 带条件
来源：http://axj.yongpay.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zta.xziqi.cn

[R50] awk 求和
来源：http://lby.yj20258888.top

awk '{s += $2} END {print s}' a.txt
来源：http://gtg.xziqi.cn

[R51] 排序去重取前几
来源：http://gud.cqqwz.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ixo.jianghu66.top

[R52] 统计行数
来源：http://ccg.hfpthk.cn

wc -l a.txt
来源：http://oyr.fzhhl.top

[R53] 查看文件头与实时尾
来源：http://lsc.ybcxt.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://igv.cashguo.top

[R54] 比较两个文件
来源：http://trn.316326.xyz

diff a.txt b.txt
来源：http://grc.yj20258888.top

[R55] 压缩与解压
来源：http://nuu.sufxvd.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dnq.zhijiandao.cn

[R56] 远程拷贝
来源：http://kbj.sxryk.cn

scp file user@host:/path/
来源：http://whd.shzxlz.cn

[R57] 远程执行命令
来源：http://wlp.xziqi.cn

ssh user@host 'uptime'
来源：http://wwe.xylfe.cn

[R58] 下载文件
来源：http://voo.havefunace.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mek.quarkkingdee.top

[R59] 发 POST JSON
来源：http://tyh.pycfn.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://duh.iojbl.cn

[R60] 只看 HTTP 状态码
来源：http://tbb.ybcxt.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sma.yangfankeji.com

[R61] 磁盘占用
来源：http://frt.hongshengwenyu.top

df -h;  du -sh *
来源：http://dih.zhixingplan.top

[R62] 找最占空间的文件
来源：http://cux.zhongyouzk.top

du -ah . | sort -rh | head -10
来源：http://lta.jiagoushi.top

[R63] 内存与进程
来源：http://llm.xuetiantiany.cn

free -h;  ps aux | grep nginx
来源：http://kbx.tian-w.cn

[R64] 结束进程
来源：http://zvz.nanxinkj.top

kill -9 $(pgrep -f app.py)
来源：http://ikh.gzhubu.top

[R65] 查看端口占用
来源：http://uzw.fktsv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://aqz.fktsv.cn

[R66] 定时任务
来源：http://jzm.gaohongyu789.top

crontab -e;  crontab -l
来源：http://cxh.wangshuangyany.cn

[R67] 生成随机十六进制串
来源：http://mle.ehwqpu.com

openssl rand -hex 16
来源：http://fum.zhiwuduotai.top

[R68] 计算文件校验值
来源：http://xlr.zhijiandao.cn

sha256sum a.txt;  md5sum a.txt
来源：http://unw.fehbvm.com

[R69] 生成随机密码
来源：http://bhe.bjfxy.top

head -c 16 /dev/urandom | base64
来源：http://agg.bjfxy.top

[R70] 时间戳与互转
来源：http://wvs.kuanghao11.cn

date +%s;  date -d @1700000000
来源：http://voa.sufxvd.cn

[R71] 日期格式化
来源：http://jzr.cdnleiting.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://lxw.chenlongwang.top

[R72] 等待端口就绪
来源：http://bjl.yonumen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://lde.xziqi.cn

[R73] 分割大日志
来源：http://cjf.jianghu66.top

split -l 1000 big.log part_
来源：http://pul.bjfxy.top

[R74] 批量重命名
来源：http://qof.smart0.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ial.pengpengdd.cyou

[R75] 导出环境变量
来源：http://jmp.ivvv.top


<!-- 参考信息 -->