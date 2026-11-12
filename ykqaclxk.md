代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://uvr.ywan-chungtsiang.top

[Q30] 分组统计
来源：http://nfd.ctjpmb.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fuo.yj20258.top

[Q31] 分组后过滤
来源：http://dtd.xziqi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wpo.ybcxt.top

[Q32] 分组拼接字符串
来源：http://jsx.daria6918.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mud.bjfxy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jys.9152youxi.cn

[Q33] 多列分组
来源：http://ndv.ctjpmb.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vrb.dashuyun.cn

[Q34] 每组取第一条
来源：http://ktf.sjlbkw.cn

SELECT * FROM (
来源：http://kov.gotoacloud.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://njs.xuetiantiany.cn

) t WHERE rn = 1;
来源：http://zzw.shuidangran.top

[Q35] 内连接
来源：http://xgr.zycfv.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zev.tian-w.cn

[Q36] 左连接
来源：http://paj.yongpay.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ukc.shangyingyoupin.top

[Q37] 右连接
来源：http://rox.pengpengdd.cyou

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zpy.fzhhl.top

[Q38] 全外连接（PostgreSQL）
来源：http://tdm.vqdsnc.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mld.jinqigufen.top

[Q39] 自连接（查上下级）
来源：http://sim.hysaishi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://tao.cheryme.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://got.yongpay.top

[Q40] 交叉连接（笛卡尔积）
来源：http://aqy.jinghuilouyu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vee.shuidangran.top

[Q41] 多表连接
来源：http://jzw.yanxiufei.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bos.ywan-chungtsiang.top

JOIN users u ON u.id = o.user_id
来源：http://vhl.zhaomingkeji.xyz

JOIN products p ON p.id = o.product_id;
来源：http://ook.jinqigufen.top

[Q42] 连接条件附加过滤
来源：http://wbx.xylfe.cn

SELECT u.name, o.amount FROM users u
来源：http://cmg.hfpthk.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ttg.yj20258.top

[Q43] 标量子查询
来源：http://zhg.fengsongda.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oyd.hfpthk.cn

[Q44] IN 子查询
来源：http://wez.cqqwz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wte.iojbl.cn

[Q45] EXISTS 判断存在
来源：http://wai.havefunace.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kmp.xylfe.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tjd.guannengcc.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wga.xuetiantiany.cn

[Q47] 与平均值比较
来源：http://ivz.feifeiyinyue.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://usb.fehbvm.com

[Q48] CTE 公用表表达式
来源：http://cvz.jqgfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vzj.yj202588.top

SELECT * FROM t WHERE c > 5;
来源：http://vha.tarul.cn

[Q49] 更新单行
来源：http://xtm.yvedp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://eih.sjlbkw.cn

[Q50] 批量更新
来源：http://clq.cheryme.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xxw.daxiang520.top

[Q51] 用子查询更新
来源：http://hpl.sysykeji.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zrz.pengpengdd.cyou

[Q52] 删除指定行
来源：http://ufi.wangdashe.top

DELETE FROM users WHERE id = 10;
来源：http://ryf.fehbvm.com

[Q53] 按条件删除
来源：http://vbi.iojbl.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mrc.aizwys.cn

[Q54] 清空表
来源：http://tms.guowangkeji.top

TRUNCATE TABLE logs;
来源：http://xlq.xinyue.icu

[Q55] 排名（并列占位）
来源：http://izf.gogol.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vkp.hnxiangtu.top

[Q56] 密集排名（并列不占位）
来源：http://wpv.chenjidiqi.icu

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zec.pycfn.com

[Q57] 行号
来源：http://xar.xinyue.icu

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tec.zhengqikj.top

[Q58] 累计求和
来源：http://jgi.vqdsnc.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wsw.jyoumei.cn

[Q59] 分组内累计
来源：http://nfe.fengsongda.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://brq.wangshuangyany.cn

[Q60] 取上一行 / 下一行
来源：http://aah.cdnleiting.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://frd.c1oappe.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ywf.c1oappe.top

[Q61] 移动平均
来源：http://oqj.guannengcc.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iey.hnxiangtu.top

[Q62] 分组占比
来源：http://udf.yangfankeji.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zlg.fengsongda.top

[Q63] 开启事务
来源：http://djm.smart0.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://rzu.316326.xyz

[Q64] 提交事务
来源：http://dzy.gzhubu.top

COMMIT;
来源：http://zwy.ybcxt.top

[Q65] 回滚事务
来源：http://qwl.shanyushiyangkeji.top

ROLLBACK;
来源：http://ari.yvedp.cn

[Q66] 行锁查询
来源：http://tbb.haohaochexian.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hhp.zycfv.cn

[Q67] 设置隔离级别
来源：http://tdv.zdqjudy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vxb.dianchejie.cn

[Q68] 保存点
来源：http://jmz.xuanzx.com

SAVEPOINT sp1;
来源：http://ubc.jqgfzy.top

ROLLBACK TO sp1;
来源：http://xxz.zhaomingkeji.xyz

[Q69] 查看执行计划
来源：http://lee.haohaochexian.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ogu.guannengcc.top

[Q70] 更新统计信息
来源：http://ofi.gogol.net.cn

ANALYZE TABLE users;
来源：http://kfy.yanxiufei.cn

[Q71] 查看建表语句
来源：http://kdk.hongshengwenyu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ewq.bbcook.cn

[Q72] 查看索引
来源：http://twj.dianchejie.cn

SHOW INDEX FROM users;
来源：http://cya.meibo888.top

[Q73] 查看表状态
来源：http://vhl.hfpthk.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mph.chenlongwang.top

[Q74] 强制使用索引
来源：http://twl.yanxiufei.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ndt.cqqwz.cn

[Q75] 日期格式化
来源：http://vtz.chenjidiqi.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tjv.shangyingyoupin.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ciq.yj20258888.top

[Q76] 按天统计
来源：http://bbq.hnqzz.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hyo.chenlongwang.top

[Q77] 时间加减
来源：http://kmf.fengsongda.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wfs.zycfv.cn

[Q78] 当前时间
来源：http://ree.gogol.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gxe.gaohongyu789.top

[Q79] 字符串拼接
来源：http://orf.jianghu66.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qou.cdnleiting.top

[Q80] 字符串截取
来源：http://klx.yonumen.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ejo.xinyue.icu

[Q81] 字符串替换
来源：http://due.wangshuangyany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://drs.nwbrower.top

[Q82] 字符长度与字节长度
来源：http://gzv.pengpengdd.cyou

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ixc.ctjpmb.com

[Q83] 大小写转换
来源：http://jeg.shanyushiyangkeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xxw.cucudq.cn

[Q84] 去除首尾空格
来源：http://kwj.jianghu66.top

SELECT TRIM(name) FROM users;
来源：http://gin.ydzc1.top

[Q85] 数值取整
来源：http://ypq.ctjpmb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gmg.sjlbkw.cn

[Q86] 读取 JSON 字段
来源：http://cjo.sxryk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jgm.ywan-chungtsiang.top

[Q87] JSON 字段做条件
来源：http://slm.cdnleiting.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sjb.xziqi.cn

[Q88] 行转列（条件聚合）
来源：http://fmo.yonumen.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qdt.fzhhl.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blc.birdmap.top

[Q89] 判断表是否存在
来源：http://auw.jianghu66.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://boz.jinghuilouyu.cn

[Q90] 生成序号列
来源：http://kyb.zhijiandao.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rwb.havefunace.top

================================================================================
来源：http://fyn.aizwys.cn

R. Bash 专题
来源：http://jqj.hammf.cn

================================================================================
来源：http://ipu.nwbrower.top

[R01] shebang 与严格模式
来源：http://wzd.9152youxi.cn

#!/usr/bin/env bash
来源：http://atu.shuidangran.top

set -euo pipefail
来源：http://xaf.yuxming.cn

[R02] 变量赋值与使用
来源：http://gmp.feifeiyinyue.top

name="Tom"; echo "$name"
来源：http://xut.wangdashe.top

[R03] 只读变量
来源：http://fkz.cheryme.top

readonly PI=3.14
来源：http://uhb.quarkkingdee.top

[R04] 位置参数
来源：http://oqs.hesvh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uwd.zdqjudy.top

[R05] 参数默认值
来源：http://snv.chenlongwang.top

name="${1:-default}"
来源：http://ywa.sweek.top

[R06] 判断命令是否存在
来源：http://hml.zdqjudy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jzs.epnwcf.com

[R07] if 判断文件
来源：http://dad.zhongyouzk.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yxl.zhixingplan.top

[R08] 数值比较
来源：http://ovt.aibaodan.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://doa.zhixingplan.top

[R09] 字符串比较
来源：http://hdi.zdbjq.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://csr.hcnkem.com

[R10] 正则匹配
来源：http://eta.gzhubu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yku.bjfxy.top

[R11] case 多分支
来源：http://hoc.jinghuilouyu.cn

case "$1" in
来源：http://ppv.yfazqb.com

start) echo "启动" ;;
来源：http://zia.jinghuilouyu.cn

stop)  echo "停止" ;;
来源：http://yhe.ctjpmb.com

*)     echo "未知命令" ;;
来源：http://eox.feifeiyinyue.top

esac
来源：http://jfh.gotoacloud.top

[R12] for 遍历文件
来源：http://rzg.wangshuangyany.cn

for f in *.txt; do echo "$f"; done
来源：http://hyu.dashuyun.cn

[R13] for 计数循环
来源：http://gmn.guannengcc.top

for i in {1..10}; do echo "$i"; done
来源：http://qyh.havefunace.top

[R14] C 风格 for
来源：http://zct.hnxiangtu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://etu.sxryk.cn

[R15] while 逐行读文件
来源：http://lud.cashguo.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jns.redwolf501.top

[R16] until 等待条件
来源：http://cdy.hesvh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wln.fengsongda.top

[R17] 数组定义与取值
来源：http://sbl.nanxinkj.top

arr=(a b c); echo "${arr[0]}"
来源：http://jhi.52xcode.cn

[R18] 遍历数组
来源：http://pmp.hywenlv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zmi.dianchejie.cn

[R19] 数组长度
来源：http://iud.yanxiufei.cn

echo "${#arr[@]}"
来源：http://epw.ivvv.top

[R20] 关联数组（字典）
来源：http://nwt.gotoacloud.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hxf.ctjpmb.com

[R21] 字符串长度
来源：http://isi.yongpay.top

echo "${#s}"
来源：http://ijh.fktsv.cn

[R22] 截取子串
来源：http://qak.ctjpmb.com

echo "${s:0:5}"
来源：http://gvw.zhijiandao.cn

[R23] 字符串替换
来源：http://xkm.cheryme.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jzt.sjlbkw.cn

[R24] 大小写转换
来源：http://xgj.mhx1999.top

echo "${s^^}"; echo "${s,,}"
来源：http://xpe.chenzaomai.com

[R25] 去后缀 / 去前缀
来源：http://hgr.hesvh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vpd.fktsv.cn

[R26] 命令替换
来源：http://qyp.jqgufenzy.top

now=$(date +%F); echo "$now"
来源：http://wyd.quarkkingdee.top

[R27] 算术展开
来源：http://jbe.nanxuanxn.top

echo $((1 + 2 * 3))
来源：http://zyc.andypj.xyz

[R28] 浮点运算
来源：http://lqg.quarkkingdee.top

echo "scale=2; 10/3" | bc
来源：http://mpm.shangyingyoupin.top

[R29] 定义函数
来源：http://ctk.guowangkeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://why.xuanzx.com

[R30] 函数返回状态码
来源：http://xqe.xziqi.cn

f() { return 0; }; f || echo "失败了"
来源：http://vtj.sjlbkw.cn

[R31] 局部变量
来源：http://czd.9152youxi.cn

f() { local x=1; echo "$x"; }
来源：http://vqg.zhaomingkeji.xyz

[R32] 参数个数校验
来源：http://cwq.yueranfly.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bfw.nwbrower.top

[R33] 捕获错误并提示行号
来源：http://min.yueranfly.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://myr.snrcjt.cn

[R34] 退出时清理
来源：http://dxm.tarul.cn

trap 'rm -f "$tmp"' EXIT
来源：http://unw.shuidangran.top

[R35] 后台执行并等待
来源：http://uge.daria6918.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xuj.hcnkem.com

[R36] 并发执行多个任务
来源：http://bkq.yuxming.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ovz.jianghu66.top

[R37] 把输出赋给变量
来源：http://mvf.haohaochexian.top

files=$(ls -1)
来源：http://sii.hammf.cn

[R38] 管道串联
来源：http://ubv.shuidangran.top

cat a.txt | grep -i error | wc -l
来源：http://fgy.nanxinkj.top

[R39] 重定向标准输出与错误
来源：http://cxb.jinghuilouyu.cn

cmd > out.log 2>&1
来源：http://tpl.guowangkeji.top

[R40] 追加写日志
来源：http://pth.jiagoushi.top

echo "log" >> out.log
来源：http://stc.chenjidiqi.icu

[R41] 丢弃输出
来源：http://yqk.havefunace.top

cmd >/dev/null 2>&1
来源：http://ees.zhongyouzk.top

[R42] 输入重定向
来源：http://yys.uphjek.com

wc -l < a.txt
来源：http://jcx.fengsongda.top

[R43] 按名字查找文件
来源：http://hzy.kuanghao11.cn

find . -name "*.log" -type f
来源：http://evl.jiagoushi.top

[R44] 按修改时间查找
来源：http://buk.feifeiyinyue.top

find . -mtime -7 -type f
来源：http://wmx.gaohongyu789.top

[R45] 批量删除
来源：http://clx.cdnleiting.top

find . -name "*.tmp" -delete
来源：http://rov.chenlongwang.top

[R46] 递归替换文件内容
来源：http://cab.jiagoushi.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lqi.0kj1m.cn

[R47] sed 单行替换
来源：http://hrx.chenjidiqi.icu

sed -i 's/foo/bar/g' a.txt
来源：http://ztf.316326.xyz

[R48] awk 取指定列
来源：http://ndz.jlsjyb.cn

awk '{print $1, $3}' a.txt
来源：http://qlc.fktsv.cn

[R49] awk 带条件
来源：http://fnf.cheryme.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gvh.jyoumei.cn

[R50] awk 求和
来源：http://sjs.xinyue.icu

awk '{s += $2} END {print s}' a.txt
来源：http://xwc.mhx1999.top

[R51] 排序去重取前几
来源：http://kik.hesvh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cog.jlsjyb.cn

[R52] 统计行数
来源：http://wdg.sxryk.cn

wc -l a.txt
来源：http://opq.zhoulong.xyz

[R53] 查看文件头与实时尾
来源：http://ndg.shzxlz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://aje.hammf.cn

[R54] 比较两个文件
来源：http://jmy.uphjek.com

diff a.txt b.txt
来源：http://ffu.zhaomingkeji.xyz

[R55] 压缩与解压
来源：http://nnk.52xcode.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zru.wangshuangyany.cn

[R56] 远程拷贝
来源：http://egk.jlsjyb.cn

scp file user@host:/path/
来源：http://wax.smart0.xyz

[R57] 远程执行命令
来源：http://bno.zhixingplan.top

ssh user@host 'uptime'
来源：http://buq.shangyingyoupin.top

[R58] 下载文件
来源：http://hmf.snrcjt.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://txs.ywan-chungtsiang.top

[R59] 发 POST JSON
来源：http://nux.tarul.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sbk.gotoacloud.top

[R60] 只看 HTTP 状态码
来源：http://bic.vqdsnc.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qyw.jqgfzy.top

[R61] 磁盘占用
来源：http://xtx.aibaodan.cn

df -h;  du -sh *
来源：http://rsd.jiagoushi.top

[R62] 找最占空间的文件
来源：http://htv.aibaodan.cn

du -ah . | sort -rh | head -10
来源：http://pjx.xylfe.cn

[R63] 内存与进程
来源：http://sxv.chenlongwang.top

free -h;  ps aux | grep nginx
来源：http://rvr.zycfv.cn

[R64] 结束进程
来源：http://xtr.shanyushiyangtech.top

kill -9 $(pgrep -f app.py)
来源：http://zzq.zhijiandao.cn

[R65] 查看端口占用
来源：http://geu.uphjek.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qrm.zycfv.cn

[R66] 定时任务
来源：http://qce.havefunace.top

crontab -e;  crontab -l
来源：http://gsi.hnxiangtu.top

[R67] 生成随机十六进制串
来源：http://jmq.chenlongwang.top

openssl rand -hex 16
来源：http://iga.nwbrower.top

[R68] 计算文件校验值
来源：http://vub.yuanzhike.top

sha256sum a.txt;  md5sum a.txt
来源：http://dnv.yfazqb.com

[R69] 生成随机密码
来源：http://zjn.tanke756.top

head -c 16 /dev/urandom | base64
来源：http://ueg.xingfuxueyuan.xyz

[R70] 时间戳与互转
来源：http://qju.ybcxt.top

date +%s;  date -d @1700000000
来源：http://scz.jinghuilouyu.cn

[R71] 日期格式化
来源：http://tyy.tianlin.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://bxm.jinqigufen.top

[R72] 等待端口就绪
来源：http://hvc.shzxlz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://owd.ydjk.org.cn

[R73] 分割大日志
来源：http://tjy.yvedp.cn

split -l 1000 big.log part_
来源：http://wab.daria6918.cn

[R74] 批量重命名
来源：http://wlx.316326.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iwg.andypj.xyz

[R75] 导出环境变量
来源：http://cdj.fzhhl.top

export PATH="$HOME/bin:$PATH"
来源：http://zyn.xziqi.cn

[R76] 使用临时文件
来源：http://ztm.zhoulong.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://haw.ydjk.org.cn

[R77] 读取用户输入
来源：http://qav.sweek.top

read -rp "请输入: " ans
来源：http://jei.zhijiandao.cn

[R78] 交互式菜单
来源：http://mmu.smart0.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://aga.aizwys.cn

[R79] 解析命令行选项
来源：http://qfo.sxryk.cn


<!-- 参考信息 -->