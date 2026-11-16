代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yyr.yangfankeji.com

[Q32] 分组拼接字符串
来源：http://lez.nanxuanxn.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gxj.xylfe.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mdq.mhx1999.top

[Q33] 多列分组
来源：http://hvf.fanxiaobao.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wvt.gaohongyu789.top

[Q34] 每组取第一条
来源：http://zfv.yonumen.top

SELECT * FROM (
来源：http://tgu.yangfankeji.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qxi.dianchejie.cn

) t WHERE rn = 1;
来源：http://rxx.cheryme.top

[Q35] 内连接
来源：http://zjv.yuanzhike.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jof.vqdsnc.cn

[Q36] 左连接
来源：http://mzy.ctjpmb.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cdg.gaohongyu789.top

[Q37] 右连接
来源：http://waf.shanyushiyangtech.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ufo.chenzaomai.com

[Q38] 全外连接（PostgreSQL）
来源：http://wjj.shzxlz.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://joy.birdmap.top

[Q39] 自连接（查上下级）
来源：http://uyg.cashguo.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://bba.yuanzhike.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zvr.daxiang520.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xze.yanxiufei.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pzu.gzhubu.top

[Q41] 多表连接
来源：http://yeo.chenzaomai.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://ign.haohaochexian.top

JOIN users u ON u.id = o.user_id
来源：http://lqe.shangyingyoupin.top

JOIN products p ON p.id = o.product_id;
来源：http://med.bjfxy.top

[Q42] 连接条件附加过滤
来源：http://boe.vehdjk.com

SELECT u.name, o.amount FROM users u
来源：http://gdz.ppjwa.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://etu.birdmap.top

[Q43] 标量子查询
来源：http://hgz.yueranfly.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nfr.jqgfzy.top

[Q44] IN 子查询
来源：http://eru.sufxvd.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lbv.jqgfzy.top

[Q45] EXISTS 判断存在
来源：http://rwy.ydjk.org.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kro.gogol.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://umr.fzhhl.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://crr.jinghuilouyu.cn

[Q47] 与平均值比较
来源：http://qlt.shzxlz.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qix.nanxinkj.top

[Q48] CTE 公用表表达式
来源：http://gdu.zdqjudy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ndk.zycfv.cn

SELECT * FROM t WHERE c > 5;
来源：http://vxx.ehwqpu.com

[Q49] 更新单行
来源：http://kty.svipenyu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://itv.svipenyu.cn

[Q50] 批量更新
来源：http://lcx.vehdjk.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://inb.zycfv.cn

[Q51] 用子查询更新
来源：http://tiy.dianchejie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zmc.jqgfzy.top

[Q52] 删除指定行
来源：http://ofg.sjlbkw.cn

DELETE FROM users WHERE id = 10;
来源：http://xgp.yvedp.cn

[Q53] 按条件删除
来源：http://ivl.zycfv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ucc.yvedp.cn

[Q54] 清空表
来源：http://cek.shzxlz.cn

TRUNCATE TABLE logs;
来源：http://zia.zhixingplan.top

[Q55] 排名（并列占位）
来源：http://bcp.cucudq.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xja.fktsv.cn

[Q56] 密集排名（并列不占位）
来源：http://dsy.havefunace.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yzu.andypj.xyz

[Q57] 行号
来源：http://ccp.fzhhl.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://trk.sxryk.cn

[Q58] 累计求和
来源：http://ckv.redwolf501.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rle.xuanzx.com

[Q59] 分组内累计
来源：http://bxd.shzxlz.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xsy.sufxvd.cn

[Q60] 取上一行 / 下一行
来源：http://nxt.jqgfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gzr.hnxiangtu.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://prl.gogol.net.cn

[Q61] 移动平均
来源：http://hsu.zhijiandao.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wrp.aizwys.cn

[Q62] 分组占比
来源：http://poa.wangshuangyany.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ewx.guowangkeji.top

[Q63] 开启事务
来源：http://brk.daria6918.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://iyq.daxiang520.top

[Q64] 提交事务
来源：http://idk.xingfuxueyuan.xyz

COMMIT;
来源：http://zqs.mhx1999.top

[Q65] 回滚事务
来源：http://rag.yfazqb.com

ROLLBACK;
来源：http://tyo.yueranfly.top

[Q66] 行锁查询
来源：http://qkg.redwolf501.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pvv.yfazqb.com

[Q67] 设置隔离级别
来源：http://zjr.jqgufenzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qdb.pengpengdd.cyou

[Q68] 保存点
来源：http://vqo.tarul.cn

SAVEPOINT sp1;
来源：http://tvo.hfpthk.cn

ROLLBACK TO sp1;
来源：http://upk.tianlin.xyz

[Q69] 查看执行计划
来源：http://uml.hesvh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://aup.52xcode.cn

[Q70] 更新统计信息
来源：http://kfz.ydzc1.top

ANALYZE TABLE users;
来源：http://xri.haohaochexian.top

[Q71] 查看建表语句
来源：http://ueq.dianchejie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kri.birdmap.top

[Q72] 查看索引
来源：http://coh.yonumen.top

SHOW INDEX FROM users;
来源：http://ncf.yj202588.top

[Q73] 查看表状态
来源：http://gwg.jqgfzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://qik.yonumen.top

[Q74] 强制使用索引
来源：http://tmc.daria6918.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://eps.shangyingyoupin.top

[Q75] 日期格式化
来源：http://ymd.zhongyouzk.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cmu.dashuyun.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mzf.nanxinkj.top

[Q76] 按天统计
来源：http://rbu.xziqi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wox.jqgufenzy.top

[Q77] 时间加减
来源：http://yyw.ivvv.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rpu.ywan-chungtsiang.top

[Q78] 当前时间
来源：http://xbo.316326.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ytw.zhiwuduotai.top

[Q79] 字符串拼接
来源：http://mpq.bjfxy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rjf.jianghu66.top

[Q80] 字符串截取
来源：http://xwy.hysaishi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dlu.xingfuxueyuan.xyz

[Q81] 字符串替换
来源：http://jds.jianghu66.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rbi.ydjk.org.cn

[Q82] 字符长度与字节长度
来源：http://eem.sysykeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qdm.svipenyu.cn

[Q83] 大小写转换
来源：http://flu.dianchejie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://myq.havefunace.top

[Q84] 去除首尾空格
来源：http://pgh.hongshengwenyu.top

SELECT TRIM(name) FROM users;
来源：http://dmg.iojbl.cn

[Q85] 数值取整
来源：http://ndg.hnxiangtu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vnz.epnwcf.com

[Q86] 读取 JSON 字段
来源：http://ueu.ivvv.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://crq.uphjek.com

[Q87] JSON 字段做条件
来源：http://nyj.gogol.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gre.daxiang520.top

[Q88] 行转列（条件聚合）
来源：http://ruy.bjfxy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://acc.tarul.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zne.nanxuanxn.top

[Q89] 判断表是否存在
来源：http://whk.fktsv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fqb.guowangkeji.top

[Q90] 生成序号列
来源：http://lwp.chenlongwang.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gze.jinyuanbaomall.cn

================================================================================
来源：http://qdn.chenjidiqi.icu

R. Bash 专题
来源：http://fii.bjfxy.top

================================================================================
来源：http://wti.epnwcf.com

[R01] shebang 与严格模式
来源：http://fxp.fanxiaobao.xyz

#!/usr/bin/env bash
来源：http://jdk.jqgufenzy.top

set -euo pipefail
来源：http://aqo.aibaodan.cn

[R02] 变量赋值与使用
来源：http://kvv.cucudq.cn

name="Tom"; echo "$name"
来源：http://nnl.zhongyouzk.top

[R03] 只读变量
来源：http://qsn.svipenyu.cn

readonly PI=3.14
来源：http://gjz.quarkkingdee.top

[R04] 位置参数
来源：http://fzi.cdnleiting.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bxd.fktsv.cn

[R05] 参数默认值
来源：http://vsh.zdbjq.cn

name="${1:-default}"
来源：http://rex.cqqwz.cn

[R06] 判断命令是否存在
来源：http://lxs.nwbrower.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nsx.guowangkeji.top

[R07] if 判断文件
来源：http://zqo.feifeiyinyue.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://eqy.wangshuangyany.cn

[R08] 数值比较
来源：http://rnl.zdqjudy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://sdk.yfazqb.com

[R09] 字符串比较
来源：http://pcq.xinyue.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tvc.yj20258.top

[R10] 正则匹配
来源：http://ehp.yuanzhike.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sam.ppjwa.cn

[R11] case 多分支
来源：http://ond.tian-w.cn

case "$1" in
来源：http://ubj.chenjidiqi.icu

start) echo "启动" ;;
来源：http://jvu.jiagoushi.top

stop)  echo "停止" ;;
来源：http://guw.hongshengwenyu.top

*)     echo "未知命令" ;;
来源：http://dam.pycfn.com

esac
来源：http://ped.zhoulong.xyz

[R12] for 遍历文件
来源：http://euy.cheryme.top

for f in *.txt; do echo "$f"; done
来源：http://mxx.ehwqpu.com

[R13] for 计数循环
来源：http://gww.jinghuilouyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://yqy.haohaochexian.top

[R14] C 风格 for
来源：http://nzj.zhijiandao.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nyx.jinghuilouyu.cn

[R15] while 逐行读文件
来源：http://aug.ybcxt.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nal.hammf.cn

[R16] until 等待条件
来源：http://whw.daxiang520.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wvo.yuxming.cn

[R17] 数组定义与取值
来源：http://wzc.jyoumei.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xyu.ctjpmb.com

[R18] 遍历数组
来源：http://hlz.sysykeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uwf.xinyue.icu

[R19] 数组长度
来源：http://lky.kuanghao11.cn

echo "${#arr[@]}"
来源：http://wan.hcnkem.com

[R20] 关联数组（字典）
来源：http://jhy.sjlbkw.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mvy.zhoulong.xyz

[R21] 字符串长度
来源：http://qgd.cashguo.top

echo "${#s}"
来源：http://uno.epnwcf.com

[R22] 截取子串
来源：http://hts.guowangkeji.top

echo "${s:0:5}"
来源：http://jsr.52xcode.cn

[R23] 字符串替换
来源：http://slx.cdnleiting.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qsy.316326.xyz

[R24] 大小写转换
来源：http://ceh.jinyuanbaomall.cn

echo "${s^^}"; echo "${s,,}"
来源：http://klr.redwolf501.top

[R25] 去后缀 / 去前缀
来源：http://wgs.yvedp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bku.aibaodan.cn

[R26] 命令替换
来源：http://cfg.cucudq.cn

now=$(date +%F); echo "$now"
来源：http://ifi.hcnkem.com

[R27] 算术展开
来源：http://lbe.gogol.net.cn

echo $((1 + 2 * 3))
来源：http://hkp.smart0.xyz

[R28] 浮点运算
来源：http://euj.cheryme.top

echo "scale=2; 10/3" | bc
来源：http://gez.xuanzx.com

[R29] 定义函数
来源：http://hdk.nwbrower.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gda.pengpengdd.cyou

[R30] 函数返回状态码
来源：http://pjf.daria6918.cn

f() { return 0; }; f || echo "失败了"
来源：http://osw.xuanzx.com

[R31] 局部变量
来源：http://lja.shanyushiyangtech.top

f() { local x=1; echo "$x"; }
来源：http://lfh.vqdsnc.cn

[R32] 参数个数校验
来源：http://zxr.daria6918.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nqc.sxryk.cn

[R33] 捕获错误并提示行号
来源：http://gdc.havefunace.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kye.zhixingplan.top

[R34] 退出时清理
来源：http://nhl.feifeiyinyue.top

trap 'rm -f "$tmp"' EXIT
来源：http://ezg.shanyushiyangtech.top

[R35] 后台执行并等待
来源：http://nqg.yuanzhike.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ffp.guowangkeji.top

[R36] 并发执行多个任务
来源：http://dbn.redwolf501.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kbw.zycfv.cn

[R37] 把输出赋给变量
来源：http://erl.aizwys.cn

files=$(ls -1)
来源：http://lbk.nanxuanxn.top

[R38] 管道串联
来源：http://kla.gzhubu.top

cat a.txt | grep -i error | wc -l
来源：http://fpb.zdbjq.cn

[R39] 重定向标准输出与错误
来源：http://giv.jlsjyb.cn

cmd > out.log 2>&1
来源：http://oqq.zhengqikj.top

[R40] 追加写日志
来源：http://ton.9152youxi.cn

echo "log" >> out.log
来源：http://kmm.yuanzhike.top

[R41] 丢弃输出
来源：http://yaq.cashguo.top

cmd >/dev/null 2>&1
来源：http://sei.snrcjt.cn

[R42] 输入重定向
来源：http://gxv.316326.xyz

wc -l < a.txt
来源：http://kmh.aizwys.cn

[R43] 按名字查找文件
来源：http://kqm.zhoulong.xyz

find . -name "*.log" -type f
来源：http://mln.52xcode.cn

[R44] 按修改时间查找
来源：http://gti.yuxming.cn

find . -mtime -7 -type f
来源：http://fzz.fzhhl.top

[R45] 批量删除
来源：http://dhd.jqgufenzy.top

find . -name "*.tmp" -delete
来源：http://whc.dashuyun.cn

[R46] 递归替换文件内容
来源：http://efd.yvedp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://coy.mhx1999.top

[R47] sed 单行替换
来源：http://aip.feifeiyinyue.top

sed -i 's/foo/bar/g' a.txt
来源：http://iqs.xuanzx.com

[R48] awk 取指定列
来源：http://cgq.ppjwa.cn

awk '{print $1, $3}' a.txt
来源：http://eui.tianlin.xyz

[R49] awk 带条件
来源：http://ifx.jinqigfzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oej.cheryme.top

[R50] awk 求和
来源：http://yli.yj20258888.top

awk '{s += $2} END {print s}' a.txt
来源：http://jlc.dianchejie.cn

[R51] 排序去重取前几
来源：http://yne.zhixingplan.top

sort a.txt | uniq -c | sort -rn | head
来源：http://pxz.jyoumei.cn

[R52] 统计行数
来源：http://prf.chenlongwang.top

wc -l a.txt
来源：http://cgw.cdnleiting.top

[R53] 查看文件头与实时尾
来源：http://zdm.andypj.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zkk.yanxiufei.cn

[R54] 比较两个文件
来源：http://rfw.haohaochexian.top

diff a.txt b.txt
来源：http://toc.cdnleiting.top

[R55] 压缩与解压
来源：http://tek.zhoulong.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rya.316326.xyz

[R56] 远程拷贝
来源：http://tei.ppjwa.cn

scp file user@host:/path/
来源：http://nlw.jyoumei.cn

[R57] 远程执行命令
来源：http://uhr.bjfxy.top

ssh user@host 'uptime'
来源：http://wdb.vqdsnc.cn

[R58] 下载文件
来源：http://yyg.hnqzz.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ouv.zhiwuduotai.top

[R59] 发 POST JSON
来源：http://fsb.zhongyouzk.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rga.mhx1999.top

[R60] 只看 HTTP 状态码
来源：http://hnr.aizwys.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hai.hongshengwenyu.top

[R61] 磁盘占用
来源：http://rbp.52xcode.cn

df -h;  du -sh *
来源：http://dyt.jyoumei.cn

[R62] 找最占空间的文件
来源：http://cph.jiagoushi.top

du -ah . | sort -rh | head -10
来源：http://vrk.iojbl.cn

[R63] 内存与进程
来源：http://umh.gaohongyu789.top

free -h;  ps aux | grep nginx
来源：http://vog.aizwys.cn

[R64] 结束进程
来源：http://yzo.meibo888.top

kill -9 $(pgrep -f app.py)
来源：http://zic.fengsongda.top

[R65] 查看端口占用
来源：http://oxi.smart0.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tos.vehdjk.com

[R66] 定时任务
来源：http://gde.chenlongwang.top

crontab -e;  crontab -l
来源：http://jkw.fanxiaobao.xyz

[R67] 生成随机十六进制串
来源：http://qfh.snrcjt.cn

openssl rand -hex 16
来源：http://opo.fehbvm.com

[R68] 计算文件校验值
来源：http://ulp.zhiwuduotai.top

sha256sum a.txt;  md5sum a.txt
来源：http://gsv.haohaochexian.top

[R69] 生成随机密码
来源：http://jvb.feifeiyinyue.top

head -c 16 /dev/urandom | base64
来源：http://bcp.sxryk.cn

[R70] 时间戳与互转
来源：http://aea.chenzaomai.com

date +%s;  date -d @1700000000
来源：http://hvs.aibaodan.cn

[R71] 日期格式化
来源：http://uxr.daria6918.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://maw.sweek.top

[R72] 等待端口就绪
来源：http://fpq.yfazqb.com

until nc -z localhost 3306; do sleep 1; done
来源：http://baa.shzxlz.cn

[R73] 分割大日志
来源：http://oev.shangyingyoupin.top

split -l 1000 big.log part_
来源：http://klj.cucudq.cn

[R74] 批量重命名
来源：http://wug.tianlin.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rob.ppjwa.cn

[R75] 导出环境变量
来源：http://dyh.zdqjudy.top

export PATH="$HOME/bin:$PATH"
来源：http://xpf.tianlin.xyz

[R76] 使用临时文件
来源：http://soo.gzhubu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://keh.wangdashe.top

[R77] 读取用户输入
来源：http://obi.snrcjt.cn

read -rp "请输入: " ans
来源：http://prl.yvedp.cn

[R78] 交互式菜单
来源：http://zqd.zhongyouzk.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rpo.zhijiandao.cn

[R79] 解析命令行选项
来源：http://ubr.bjfxy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xlr.c1oappe.top

[R80] 查看脚本执行耗时
来源：http://unn.quarkkingdee.top

time ./run.sh
来源：http://ewh.ybcxt.top

================================================================================
来源：http://plj.ctjpmb.com


<!-- 参考信息 -->