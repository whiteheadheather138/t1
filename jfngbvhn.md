代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://cid.fanxiaobao.xyz

[Q30] 分组统计
来源：http://mng.sweek.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xet.jinqigfzy.top

[Q31] 分组后过滤
来源：http://xka.pengpengdd.cyou

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ddz.jinghuilouyu.cn

[Q32] 分组拼接字符串
来源：http://omj.sjlbkw.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hqo.fzhhl.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gcm.hcnkem.com

[Q33] 多列分组
来源：http://saj.jqgfzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lwi.epnwcf.com

[Q34] 每组取第一条
来源：http://yho.tianlin.xyz

SELECT * FROM (
来源：http://owv.meibo888.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tzm.sweek.top

) t WHERE rn = 1;
来源：http://prn.daria6918.cn

[Q35] 内连接
来源：http://lqs.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wxd.kuanghao11.cn

[Q36] 左连接
来源：http://xlj.smart0.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bsi.xziqi.cn

[Q37] 右连接
来源：http://idz.ydzc1.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://whq.cashguo.top

[Q38] 全外连接（PostgreSQL）
来源：http://pal.gogol.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tbp.svipenyu.cn

[Q39] 自连接（查上下级）
来源：http://orh.vqdsnc.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://juo.zhoulong.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jop.hcnkem.com

[Q40] 交叉连接（笛卡尔积）
来源：http://ncp.shzxlz.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://noa.dianchejie.cn

[Q41] 多表连接
来源：http://tht.tian-w.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://inl.shanyushiyangtech.top

JOIN users u ON u.id = o.user_id
来源：http://gnq.nanxuanxn.top

JOIN products p ON p.id = o.product_id;
来源：http://tsm.c1oappe.top

[Q42] 连接条件附加过滤
来源：http://wtv.smart0.xyz

SELECT u.name, o.amount FROM users u
来源：http://leu.yfazqb.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://imd.chenjidiqi.icu

[Q43] 标量子查询
来源：http://pfd.shangyingyoupin.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://owf.yuanzhike.top

[Q44] IN 子查询
来源：http://dzp.feifeiyinyue.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ceu.shuidangran.top

[Q45] EXISTS 判断存在
来源：http://cfs.hysaishi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://via.zhengqikj.top

[Q46] NOT EXISTS 判断不存在
来源：http://emv.epnwcf.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://izc.jqgufenzy.top

[Q47] 与平均值比较
来源：http://tep.ivvv.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jqr.fengsongda.top

[Q48] CTE 公用表表达式
来源：http://rrp.jqgfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rlo.zhixingplan.top

SELECT * FROM t WHERE c > 5;
来源：http://tdc.xziqi.cn

[Q49] 更新单行
来源：http://bfg.cdnleiting.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://glk.0kj1m.cn

[Q50] 批量更新
来源：http://dls.nanxinkj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wcu.jinghuilouyu.cn

[Q51] 用子查询更新
来源：http://ywz.zhoulong.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qkt.uphjek.com

[Q52] 删除指定行
来源：http://nmk.havefunace.top

DELETE FROM users WHERE id = 10;
来源：http://rli.yj20258.top

[Q53] 按条件删除
来源：http://oxn.andypj.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://olt.nwbrower.top

[Q54] 清空表
来源：http://wzq.zhijiandao.cn

TRUNCATE TABLE logs;
来源：http://beb.jinqigfzy.top

[Q55] 排名（并列占位）
来源：http://oqm.tianlin.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ayp.hysaishi.cn

[Q56] 密集排名（并列不占位）
来源：http://viy.jinqigufen.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://obp.zycfv.cn

[Q57] 行号
来源：http://nru.ydjk.org.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://muc.hfpthk.cn

[Q58] 累计求和
来源：http://tct.9152youxi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ftw.hywenlv.cn

[Q59] 分组内累计
来源：http://zkf.jinqigfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://npw.bjfxy.top

[Q60] 取上一行 / 下一行
来源：http://nmf.jyoumei.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ejn.smart0.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://axe.haohaochexian.top

[Q61] 移动平均
来源：http://hil.hcnkem.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ltl.zhengqikj.top

[Q62] 分组占比
来源：http://lqx.chenjidiqi.icu

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cpf.zycfv.cn

[Q63] 开启事务
来源：http://syi.zhaomingkeji.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://asr.ivvv.top

[Q64] 提交事务
来源：http://sor.yanxiufei.cn

COMMIT;
来源：http://vsq.andypj.xyz

[Q65] 回滚事务
来源：http://rqd.ybcxt.top

ROLLBACK;
来源：http://aqv.bbcook.cn

[Q66] 行锁查询
来源：http://gnb.yj20258888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pjd.hesvh.cn

[Q67] 设置隔离级别
来源：http://pwp.yj20258888.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dfg.vehdjk.com

[Q68] 保存点
来源：http://ozf.feifeiyinyue.top

SAVEPOINT sp1;
来源：http://ius.feifeiyinyue.top

ROLLBACK TO sp1;
来源：http://txb.jiagoushi.top

[Q69] 查看执行计划
来源：http://chq.sweek.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kdu.yuanzhike.top

[Q70] 更新统计信息
来源：http://and.jinyuanbaomall.cn

ANALYZE TABLE users;
来源：http://mem.hnqzz.top

[Q71] 查看建表语句
来源：http://dvi.chenzaomai.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dzf.hysaishi.cn

[Q72] 查看索引
来源：http://nvz.jyoumei.cn

SHOW INDEX FROM users;
来源：http://kcl.tarul.cn

[Q73] 查看表状态
来源：http://rbk.guowangkeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ahp.hysaishi.cn

[Q74] 强制使用索引
来源：http://dwe.pycfn.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kag.zycfv.cn

[Q75] 日期格式化
来源：http://sil.hongshengwenyu.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nbp.gaohongyu789.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fyy.yvedp.cn

[Q76] 按天统计
来源：http://hvv.mhx1999.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gam.shanyushiyangtech.top

[Q77] 时间加减
来源：http://iol.pengpengdd.cyou

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ygx.birdmap.top

[Q78] 当前时间
来源：http://sdx.shanyushiyangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mtt.wangshuangyany.cn

[Q79] 字符串拼接
来源：http://llq.jlsjyb.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qwm.52xcode.cn

[Q80] 字符串截取
来源：http://zcl.fehbvm.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ktx.havefunace.top

[Q81] 字符串替换
来源：http://bqg.havefunace.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gyp.cqqwz.cn

[Q82] 字符长度与字节长度
来源：http://tic.yj20258888.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mil.havefunace.top

[Q83] 大小写转换
来源：http://tym.feifeiyinyue.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kpy.hywenlv.cn

[Q84] 去除首尾空格
来源：http://bwo.xingfuxueyuan.xyz

SELECT TRIM(name) FROM users;
来源：http://xne.yueranfly.top

[Q85] 数值取整
来源：http://ads.ppjwa.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zkg.hfpthk.cn

[Q86] 读取 JSON 字段
来源：http://fsi.andypj.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://app.uphjek.com

[Q87] JSON 字段做条件
来源：http://htf.9152youxi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cpu.9152youxi.cn

[Q88] 行转列（条件聚合）
来源：http://efs.quarkkingdee.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://huo.xinyue.icu

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lah.cucudq.cn

[Q89] 判断表是否存在
来源：http://jmc.ivvv.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bpk.zycfv.cn

[Q90] 生成序号列
来源：http://cwg.yfazqb.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://olx.fengsongda.top

================================================================================
来源：http://toh.chenlongwang.top

R. Bash 专题
来源：http://ymx.smart0.xyz

================================================================================
来源：http://oof.shuidangran.top

[R01] shebang 与严格模式
来源：http://pjp.yongpay.top

#!/usr/bin/env bash
来源：http://rog.ybcxt.top

set -euo pipefail
来源：http://pqp.aizwys.cn

[R02] 变量赋值与使用
来源：http://oog.jiagoushi.top

name="Tom"; echo "$name"
来源：http://dlo.xuanzx.com

[R03] 只读变量
来源：http://eon.wangshuangyany.cn

readonly PI=3.14
来源：http://pbr.sysykeji.top

[R04] 位置参数
来源：http://lbk.haohaochexian.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tid.guannengcc.top

[R05] 参数默认值
来源：http://tvn.pengpengdd.cyou

name="${1:-default}"
来源：http://ktg.jinqigfzy.top

[R06] 判断命令是否存在
来源：http://qud.cdnleiting.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lip.havefunace.top

[R07] if 判断文件
来源：http://wkg.zycfv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://avo.tarul.cn

[R08] 数值比较
来源：http://fjh.sjlbkw.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sxw.hfpthk.cn

[R09] 字符串比较
来源：http://ctm.52xcode.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://otv.gogol.net.cn

[R10] 正则匹配
来源：http://nzx.pycfn.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ecx.pengpengdd.cyou

[R11] case 多分支
来源：http://esi.fktsv.cn

case "$1" in
来源：http://gfm.tianlin.xyz

start) echo "启动" ;;
来源：http://xtf.havefunace.top

stop)  echo "停止" ;;
来源：http://jko.zdbjq.cn

*)     echo "未知命令" ;;
来源：http://dwb.xingfuxueyuan.xyz

esac
来源：http://sfz.jiagoushi.top

[R12] for 遍历文件
来源：http://stb.yj20258888.top

for f in *.txt; do echo "$f"; done
来源：http://inz.jqgfzy.top

[R13] for 计数循环
来源：http://ehe.jyoumei.cn

for i in {1..10}; do echo "$i"; done
来源：http://cvs.yfazqb.com

[R14] C 风格 for
来源：http://xpm.zhengqikj.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fxw.fengsongda.top

[R15] while 逐行读文件
来源：http://bpn.cheryme.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bwd.52xcode.cn

[R16] until 等待条件
来源：http://hwl.tianlin.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kat.guannengcc.top

[R17] 数组定义与取值
来源：http://pux.guannengcc.top

arr=(a b c); echo "${arr[0]}"
来源：http://bxm.hcnkem.com

[R18] 遍历数组
来源：http://aei.xingfuxueyuan.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bba.nwbrower.top

[R19] 数组长度
来源：http://nft.mhx1999.top

echo "${#arr[@]}"
来源：http://hcx.pycfn.com

[R20] 关联数组（字典）
来源：http://uqa.jiagoushi.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://edf.tarul.cn

[R21] 字符串长度
来源：http://hbm.xziqi.cn

echo "${#s}"
来源：http://svb.cdnleiting.top

[R22] 截取子串
来源：http://dsv.jinyuanbaomall.cn

echo "${s:0:5}"
来源：http://vlm.chenjidiqi.icu

[R23] 字符串替换
来源：http://hkm.nanxinkj.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jff.xingfuxueyuan.xyz

[R24] 大小写转换
来源：http://jpr.cheryme.top

echo "${s^^}"; echo "${s,,}"
来源：http://css.zdqjudy.top

[R25] 去后缀 / 去前缀
来源：http://cfq.sufxvd.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dda.tarul.cn

[R26] 命令替换
来源：http://wkp.sweek.top

now=$(date +%F); echo "$now"
来源：http://cwm.aibaodan.cn

[R27] 算术展开
来源：http://wom.zhoulong.xyz

echo $((1 + 2 * 3))
来源：http://zwo.yangfankeji.com

[R28] 浮点运算
来源：http://mok.jinyuanbaomall.cn

echo "scale=2; 10/3" | bc
来源：http://ggj.jiagoushi.top

[R29] 定义函数
来源：http://uvw.andypj.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://acf.yangfankeji.com

[R30] 函数返回状态码
来源：http://isb.hnqzz.top

f() { return 0; }; f || echo "失败了"
来源：http://knf.hcnkem.com

[R31] 局部变量
来源：http://jfi.fktsv.cn

f() { local x=1; echo "$x"; }
来源：http://tpr.cashguo.top

[R32] 参数个数校验
来源：http://jos.zycfv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yam.fehbvm.com

[R33] 捕获错误并提示行号
来源：http://stq.ivvv.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uen.daxiang520.top

[R34] 退出时清理
来源：http://jfz.nanxuanxn.top

trap 'rm -f "$tmp"' EXIT
来源：http://asn.hesvh.cn

[R35] 后台执行并等待
来源：http://ddp.xylfe.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://psi.xingfuxueyuan.xyz

[R36] 并发执行多个任务
来源：http://mum.pengpengdd.cyou

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bph.zhoulong.xyz

[R37] 把输出赋给变量
来源：http://tdc.ybcxt.top

files=$(ls -1)
来源：http://ufn.ydzc1.top

[R38] 管道串联
来源：http://zjs.tanke756.top

cat a.txt | grep -i error | wc -l
来源：http://qlw.sxryk.cn

[R39] 重定向标准输出与错误
来源：http://sxm.hongshengwenyu.top

cmd > out.log 2>&1
来源：http://tok.zycfv.cn

[R40] 追加写日志
来源：http://zna.nanxinkj.top

echo "log" >> out.log
来源：http://odv.feifeiyinyue.top

[R41] 丢弃输出
来源：http://xxj.yueranfly.top

cmd >/dev/null 2>&1
来源：http://ewn.guowangkeji.top

[R42] 输入重定向
来源：http://emk.feifeiyinyue.top

wc -l < a.txt
来源：http://zxx.daxiang520.top

[R43] 按名字查找文件
来源：http://plz.yj20258888.top

find . -name "*.log" -type f
来源：http://mot.gogol.net.cn

[R44] 按修改时间查找
来源：http://suz.haohaochexian.top

find . -mtime -7 -type f
来源：http://cyl.yangfankeji.com

[R45] 批量删除
来源：http://iuo.nwbrower.top

find . -name "*.tmp" -delete
来源：http://pnd.jqgfzy.top

[R46] 递归替换文件内容
来源：http://uaa.hywenlv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pia.pengpengdd.cyou

[R47] sed 单行替换
来源：http://ymj.zhijiandao.cn

sed -i 's/foo/bar/g' a.txt
来源：http://oyj.hcnkem.com

[R48] awk 取指定列
来源：http://tie.zhoulong.xyz

awk '{print $1, $3}' a.txt
来源：http://mrp.fanxiaobao.xyz

[R49] awk 带条件
来源：http://xdc.fzhhl.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fni.ehwqpu.com

[R50] awk 求和
来源：http://dij.yfazqb.com

awk '{s += $2} END {print s}' a.txt
来源：http://qci.guannengcc.top

[R51] 排序去重取前几
来源：http://auf.snrcjt.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tgo.aibaodan.cn

[R52] 统计行数
来源：http://zoz.wangshuangyany.cn

wc -l a.txt
来源：http://gkr.ehwqpu.com

[R53] 查看文件头与实时尾
来源：http://rma.tian-w.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sex.chenjidiqi.icu

[R54] 比较两个文件
来源：http://ppx.tarul.cn

diff a.txt b.txt
来源：http://qtt.ppjwa.cn

[R55] 压缩与解压
来源：http://abp.shanyushiyangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jkw.cdnleiting.top

[R56] 远程拷贝
来源：http://cpc.cucudq.cn

scp file user@host:/path/
来源：http://hss.316326.xyz

[R57] 远程执行命令
来源：http://wir.0kj1m.cn

ssh user@host 'uptime'
来源：http://xct.jqgfzy.top

[R58] 下载文件
来源：http://jzj.cashguo.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://liy.nanxuanxn.top

[R59] 发 POST JSON
来源：http://ptg.xylfe.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xwo.andypj.xyz

[R60] 只看 HTTP 状态码
来源：http://rrj.jqgufenzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ace.ywan-chungtsiang.top

[R61] 磁盘占用
来源：http://ewm.zhongyouzk.top

df -h;  du -sh *
来源：http://vhm.hammf.cn

[R62] 找最占空间的文件
来源：http://kgo.hywenlv.cn

du -ah . | sort -rh | head -10
来源：http://cbn.jianghu66.top

[R63] 内存与进程
来源：http://zxu.sysykeji.top

free -h;  ps aux | grep nginx
来源：http://ayi.yangfankeji.com

[R64] 结束进程
来源：http://lkd.ydzc1.top

kill -9 $(pgrep -f app.py)
来源：http://ray.xuanzx.com

[R65] 查看端口占用
来源：http://fgi.bjfxy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sip.jinqigfzy.top

[R66] 定时任务
来源：http://hkq.gotoacloud.top

crontab -e;  crontab -l
来源：http://uay.0kj1m.cn

[R67] 生成随机十六进制串
来源：http://zzo.hongshengwenyu.top

openssl rand -hex 16
来源：http://vnv.sxryk.cn

[R68] 计算文件校验值
来源：http://gmy.xuanzx.com

sha256sum a.txt;  md5sum a.txt
来源：http://gwd.snrcjt.cn

[R69] 生成随机密码
来源：http://atf.tian-w.cn

head -c 16 /dev/urandom | base64
来源：http://wig.fanxiaobao.xyz

[R70] 时间戳与互转
来源：http://ohg.hammf.cn

date +%s;  date -d @1700000000
来源：http://yyr.gaohongyu789.top

[R71] 日期格式化
来源：http://kuc.aibaodan.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jmq.xinyue.icu

[R72] 等待端口就绪
来源：http://ruc.redwolf501.top

until nc -z localhost 3306; do sleep 1; done
来源：http://rtc.snrcjt.cn

[R73] 分割大日志
来源：http://ter.fzhhl.top

split -l 1000 big.log part_
来源：http://qut.wangshuangyany.cn

[R74] 批量重命名
来源：http://jbr.yanxiufei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fum.9152youxi.cn

[R75] 导出环境变量
来源：http://uql.kuanghao11.cn

export PATH="$HOME/bin:$PATH"
来源：http://vhv.hammf.cn

[R76] 使用临时文件
来源：http://eta.ywan-chungtsiang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mkv.0kj1m.cn

[R77] 读取用户输入
来源：http://nlv.zhaomingkeji.xyz

read -rp "请输入: " ans
来源：http://jew.ybcxt.top

[R78] 交互式菜单
来源：http://jxz.hnxiangtu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://iuu.meibo888.top

[R79] 解析命令行选项
来源：http://ctf.yj20258.top


<!-- 参考信息 -->