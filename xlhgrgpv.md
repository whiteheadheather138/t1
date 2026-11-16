代发 wailian999

[Q36] 左连接
来源：http://edm.xingfuxueyuan.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gir.yj202588.top

[Q37] 右连接
来源：http://gcr.epnwcf.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://anm.vqdsnc.cn

[Q38] 全外连接（PostgreSQL）
来源：http://nrq.shanyushiyangkeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ejj.feifeiyinyue.top

[Q39] 自连接（查上下级）
来源：http://ndu.jqgufenzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://cti.shanyushiyangkeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nfz.andypj.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://err.guowangkeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://chm.zhoulong.xyz

[Q41] 多表连接
来源：http://xff.jlsjyb.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jbq.feifeiyinyue.top

JOIN users u ON u.id = o.user_id
来源：http://dpp.kuanghao11.cn

JOIN products p ON p.id = o.product_id;
来源：http://okm.vqdsnc.cn

[Q42] 连接条件附加过滤
来源：http://prh.cdnleiting.top

SELECT u.name, o.amount FROM users u
来源：http://skl.ywan-chungtsiang.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://shs.dianchejie.cn

[Q43] 标量子查询
来源：http://rbe.c1oappe.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mui.wangshuangyany.cn

[Q44] IN 子查询
来源：http://lif.fehbvm.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ivu.gaohongyu789.top

[Q45] EXISTS 判断存在
来源：http://zql.52xcode.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pbh.sjlbkw.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gmd.havefunace.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://agh.aibaodan.cn

[Q47] 与平均值比较
来源：http://gwu.smart0.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sdb.zdqjudy.top

[Q48] CTE 公用表表达式
来源：http://nih.hysaishi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qby.ydjk.org.cn

SELECT * FROM t WHERE c > 5;
来源：http://wre.jiagoushi.top

[Q49] 更新单行
来源：http://wab.nanxinkj.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uvw.redwolf501.top

[Q50] 批量更新
来源：http://hdk.yfazqb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gfm.gotoacloud.top

[Q51] 用子查询更新
来源：http://ymi.jlsjyb.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jlr.bjfxy.top

[Q52] 删除指定行
来源：http://jyf.dianchejie.cn

DELETE FROM users WHERE id = 10;
来源：http://vru.chenlongwang.top

[Q53] 按条件删除
来源：http://egx.sweek.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hwf.daxiang520.top

[Q54] 清空表
来源：http://srq.jianghu66.top

TRUNCATE TABLE logs;
来源：http://wpg.aizwys.cn

[Q55] 排名（并列占位）
来源：http://ahd.ydzc1.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://spj.ctjpmb.com

[Q56] 密集排名（并列不占位）
来源：http://vfk.jyoumei.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nrp.cheryme.top

[Q57] 行号
来源：http://klw.shuidangran.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bys.daxiang520.top

[Q58] 累计求和
来源：http://vkl.hnxiangtu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uib.iojbl.cn

[Q59] 分组内累计
来源：http://gjp.zhongyouzk.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://unv.jyoumei.cn

[Q60] 取上一行 / 下一行
来源：http://eks.aibaodan.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uzk.kuanghao11.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ord.wangdashe.top

[Q61] 移动平均
来源：http://ufp.52xcode.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://soa.dashuyun.cn

[Q62] 分组占比
来源：http://ele.bjfxy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://usb.zhaomingkeji.xyz

[Q63] 开启事务
来源：http://kmr.nwbrower.top

START TRANSACTION;                -- 或 BEGIN
来源：http://cdx.sjlbkw.cn

[Q64] 提交事务
来源：http://pgi.haohaochexian.top

COMMIT;
来源：http://kxr.xuanzx.com

[Q65] 回滚事务
来源：http://pyz.hongshengwenyu.top

ROLLBACK;
来源：http://jlm.uphjek.com

[Q66] 行锁查询
来源：http://ylz.bjfxy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cfv.sysykeji.top

[Q67] 设置隔离级别
来源：http://mmg.nwbrower.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kbn.xinyue.icu

[Q68] 保存点
来源：http://jow.cashguo.top

SAVEPOINT sp1;
来源：http://ffr.ywan-chungtsiang.top

ROLLBACK TO sp1;
来源：http://jbc.jinghuilouyu.cn

[Q69] 查看执行计划
来源：http://sbl.smart0.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://eid.zhoulong.xyz

[Q70] 更新统计信息
来源：http://rso.yj20258888.top

ANALYZE TABLE users;
来源：http://fvp.ehwqpu.com

[Q71] 查看建表语句
来源：http://vyk.cheryme.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nvm.redwolf501.top

[Q72] 查看索引
来源：http://gsg.chenlongwang.top

SHOW INDEX FROM users;
来源：http://izo.hcnkem.com

[Q73] 查看表状态
来源：http://vdn.9152youxi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ahc.zdbjq.cn

[Q74] 强制使用索引
来源：http://nlk.dianchejie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fus.nanxuanxn.top

[Q75] 日期格式化
来源：http://rxp.tianlin.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://idb.guowangkeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zrh.zhiwuduotai.top

[Q76] 按天统计
来源：http://arx.9152youxi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vjp.havefunace.top

[Q77] 时间加减
来源：http://asn.guowangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kkc.cashguo.top

[Q78] 当前时间
来源：http://ybs.xylfe.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cbq.chenlongwang.top

[Q79] 字符串拼接
来源：http://uha.ydzc1.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ipu.nanxuanxn.top

[Q80] 字符串截取
来源：http://thx.zycfv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vnv.c1oappe.top

[Q81] 字符串替换
来源：http://tfi.svipenyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pmf.hnxiangtu.top

[Q82] 字符长度与字节长度
来源：http://qzi.jyoumei.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rdp.nwbrower.top

[Q83] 大小写转换
来源：http://xtu.yj202588.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fik.kuanghao11.cn

[Q84] 去除首尾空格
来源：http://jpe.fanxiaobao.xyz

SELECT TRIM(name) FROM users;
来源：http://ley.shanyushiyangtech.top

[Q85] 数值取整
来源：http://cwd.52xcode.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sfx.shangyingyoupin.top

[Q86] 读取 JSON 字段
来源：http://aut.gotoacloud.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fsc.shuidangran.top

[Q87] JSON 字段做条件
来源：http://xsr.jinqigfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ijt.cdnleiting.top

[Q88] 行转列（条件聚合）
来源：http://biq.hysaishi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kbs.ydjk.org.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zoq.tianlin.xyz

[Q89] 判断表是否存在
来源：http://swp.ybcxt.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zzs.haohaochexian.top

[Q90] 生成序号列
来源：http://don.ywan-chungtsiang.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wpm.andypj.xyz

================================================================================
来源：http://gta.yuanzhike.top

R. Bash 专题
来源：http://fbd.ywan-chungtsiang.top

================================================================================
来源：http://pya.dianchejie.cn

[R01] shebang 与严格模式
来源：http://ldi.zhongyouzk.top

#!/usr/bin/env bash
来源：http://ckp.jqgufenzy.top

set -euo pipefail
来源：http://ojy.snrcjt.cn

[R02] 变量赋值与使用
来源：http://zfd.epnwcf.com

name="Tom"; echo "$name"
来源：http://mxm.pycfn.com

[R03] 只读变量
来源：http://zsu.hongshengwenyu.top

readonly PI=3.14
来源：http://vzw.zhengqikj.top

[R04] 位置参数
来源：http://urx.guannengcc.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lxe.yueranfly.top

[R05] 参数默认值
来源：http://bmz.zdqjudy.top

name="${1:-default}"
来源：http://hqv.gogol.net.cn

[R06] 判断命令是否存在
来源：http://wyl.zdbjq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://aoi.havefunace.top

[R07] if 判断文件
来源：http://mtr.hfpthk.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wiw.snrcjt.cn

[R08] 数值比较
来源：http://jqr.gotoacloud.top

if (( a > b )); then echo "a 更大"; fi
来源：http://dbk.yj20258888.top

[R09] 字符串比较
来源：http://wvq.wangdashe.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nms.xziqi.cn

[R10] 正则匹配
来源：http://enm.epnwcf.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://aof.yuxming.cn

[R11] case 多分支
来源：http://lxa.zycfv.cn

case "$1" in
来源：http://pth.zhixingplan.top

start) echo "启动" ;;
来源：http://oor.yvedp.cn

stop)  echo "停止" ;;
来源：http://zis.ybcxt.top

*)     echo "未知命令" ;;
来源：http://pep.nanxinkj.top

esac
来源：http://ezb.dashuyun.cn

[R12] for 遍历文件
来源：http://enc.aibaodan.cn

for f in *.txt; do echo "$f"; done
来源：http://kal.xylfe.cn

[R13] for 计数循环
来源：http://vpm.ybcxt.top

for i in {1..10}; do echo "$i"; done
来源：http://whx.ctjpmb.com

[R14] C 风格 for
来源：http://vmj.cucudq.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pxm.xinyue.icu

[R15] while 逐行读文件
来源：http://icb.zhaomingkeji.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ugh.pengpengdd.cyou

[R16] until 等待条件
来源：http://ocu.ydzc1.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zlj.zhengqikj.top

[R17] 数组定义与取值
来源：http://noo.xylfe.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gqj.yangfankeji.com

[R18] 遍历数组
来源：http://fvz.zhongyouzk.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://izh.fktsv.cn

[R19] 数组长度
来源：http://fsv.ctjpmb.com

echo "${#arr[@]}"
来源：http://aky.fehbvm.com

[R20] 关联数组（字典）
来源：http://odf.guowangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mlt.yangfankeji.com

[R21] 字符串长度
来源：http://ucz.chenlongwang.top

echo "${#s}"
来源：http://vpj.aibaodan.cn

[R22] 截取子串
来源：http://oep.havefunace.top

echo "${s:0:5}"
来源：http://wmf.wangshuangyany.cn

[R23] 字符串替换
来源：http://zqy.andypj.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bbh.chenjidiqi.icu

[R24] 大小写转换
来源：http://dby.sxryk.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cai.hammf.cn

[R25] 去后缀 / 去前缀
来源：http://vqb.aizwys.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://alb.feifeiyinyue.top

[R26] 命令替换
来源：http://spe.jinqigufen.top

now=$(date +%F); echo "$now"
来源：http://gky.nwbrower.top

[R27] 算术展开
来源：http://eyy.bbcook.cn

echo $((1 + 2 * 3))
来源：http://qri.jinqigfzy.top

[R28] 浮点运算
来源：http://lvj.316326.xyz

echo "scale=2; 10/3" | bc
来源：http://fxw.fehbvm.com

[R29] 定义函数
来源：http://awq.dashuyun.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gct.0kj1m.cn

[R30] 函数返回状态码
来源：http://kxv.cdnleiting.top

f() { return 0; }; f || echo "失败了"
来源：http://lzr.kuanghao11.cn

[R31] 局部变量
来源：http://lob.cdnleiting.top

f() { local x=1; echo "$x"; }
来源：http://bab.havefunace.top

[R32] 参数个数校验
来源：http://pnq.tianlin.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ecs.nanxinkj.top

[R33] 捕获错误并提示行号
来源：http://pjq.yuanzhike.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kzu.sweek.top

[R34] 退出时清理
来源：http://uxj.cashguo.top

trap 'rm -f "$tmp"' EXIT
来源：http://olx.jlsjyb.cn

[R35] 后台执行并等待
来源：http://pjl.fzhhl.top

sleep 5 & pid=$!; wait "$pid"
来源：http://lrm.haohaochexian.top

[R36] 并发执行多个任务
来源：http://rhf.guannengcc.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dmp.jinyuanbaomall.cn

[R37] 把输出赋给变量
来源：http://ubn.jqgfzy.top

files=$(ls -1)
来源：http://pad.tanke756.top

[R38] 管道串联
来源：http://bhw.yongpay.top

cat a.txt | grep -i error | wc -l
来源：http://xgp.quarkkingdee.top

[R39] 重定向标准输出与错误
来源：http://msr.ybcxt.top

cmd > out.log 2>&1
来源：http://gmn.gzhubu.top

[R40] 追加写日志
来源：http://ffd.ivvv.top

echo "log" >> out.log
来源：http://nmg.havefunace.top

[R41] 丢弃输出
来源：http://txv.haohaochexian.top

cmd >/dev/null 2>&1
来源：http://tdi.quarkkingdee.top

[R42] 输入重定向
来源：http://bkk.316326.xyz

wc -l < a.txt
来源：http://err.ehwqpu.com

[R43] 按名字查找文件
来源：http://mhi.zhaomingkeji.xyz

find . -name "*.log" -type f
来源：http://hyi.nwbrower.top

[R44] 按修改时间查找
来源：http://rev.fehbvm.com

find . -mtime -7 -type f
来源：http://wss.cashguo.top

[R45] 批量删除
来源：http://mhb.jlsjyb.cn

find . -name "*.tmp" -delete
来源：http://xbv.chenjidiqi.icu

[R46] 递归替换文件内容
来源：http://hpr.xinyue.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nvp.wangdashe.top

[R47] sed 单行替换
来源：http://mdw.pengpengdd.cyou

sed -i 's/foo/bar/g' a.txt
来源：http://pfs.c1oappe.top

[R48] awk 取指定列
来源：http://imp.yonumen.top

awk '{print $1, $3}' a.txt
来源：http://tat.fktsv.cn

[R49] awk 带条件
来源：http://tci.jyoumei.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ztx.zhoulong.xyz

[R50] awk 求和
来源：http://adf.smart0.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://zma.bjfxy.top

[R51] 排序去重取前几
来源：http://pkf.nanxinkj.top

sort a.txt | uniq -c | sort -rn | head
来源：http://tyr.shangyingyoupin.top

[R52] 统计行数
来源：http://aos.yj20258.top

wc -l a.txt
来源：http://gwr.uphjek.com

[R53] 查看文件头与实时尾
来源：http://bfd.zdbjq.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vsw.yongpay.top

[R54] 比较两个文件
来源：http://dwz.wangdashe.top

diff a.txt b.txt
来源：http://okz.fengsongda.top

[R55] 压缩与解压
来源：http://ako.yj20258888.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gdk.mhx1999.top

[R56] 远程拷贝
来源：http://ilx.feifeiyinyue.top

scp file user@host:/path/
来源：http://uji.aibaodan.cn

[R57] 远程执行命令
来源：http://xfl.shanyushiyangtech.top

ssh user@host 'uptime'
来源：http://sbl.hcnkem.com

[R58] 下载文件
来源：http://uln.shuidangran.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pib.dashuyun.cn

[R59] 发 POST JSON
来源：http://ssk.mhx1999.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jjz.yuanzhike.top

[R60] 只看 HTTP 状态码
来源：http://ujr.mhx1999.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rcc.sjlbkw.cn

[R61] 磁盘占用
来源：http://fks.birdmap.top

df -h;  du -sh *
来源：http://axw.zhengqikj.top

[R62] 找最占空间的文件
来源：http://lee.iojbl.cn

du -ah . | sort -rh | head -10
来源：http://caa.ydjk.org.cn

[R63] 内存与进程
来源：http://ubw.svipenyu.cn

free -h;  ps aux | grep nginx
来源：http://tjg.jyoumei.cn

[R64] 结束进程
来源：http://oaz.fzhhl.top

kill -9 $(pgrep -f app.py)
来源：http://iue.ydzc1.top

[R65] 查看端口占用
来源：http://axp.zdbjq.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://upt.sufxvd.cn

[R66] 定时任务
来源：http://mln.xziqi.cn

crontab -e;  crontab -l
来源：http://cor.sysykeji.top

[R67] 生成随机十六进制串
来源：http://ksf.jinyuanbaomall.cn

openssl rand -hex 16
来源：http://vqw.sysykeji.top

[R68] 计算文件校验值
来源：http://fic.zycfv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zra.hesvh.cn

[R69] 生成随机密码
来源：http://dkb.tian-w.cn

head -c 16 /dev/urandom | base64
来源：http://afq.zhongyouzk.top

[R70] 时间戳与互转
来源：http://kll.jinyuanbaomall.cn

date +%s;  date -d @1700000000
来源：http://txo.chenzaomai.com

[R71] 日期格式化
来源：http://sry.chenjidiqi.icu

date +"%Y-%m-%d %H:%M:%S"
来源：http://zgi.jinghuilouyu.cn

[R72] 等待端口就绪
来源：http://isb.shanyushiyangkeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nfs.yuanzhike.top

[R73] 分割大日志
来源：http://nwm.tianlin.xyz

split -l 1000 big.log part_
来源：http://cqs.jinqigufen.top

[R74] 批量重命名
来源：http://prm.shzxlz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rtp.guowangkeji.top

[R75] 导出环境变量
来源：http://zse.bjfxy.top

export PATH="$HOME/bin:$PATH"
来源：http://hxo.redwolf501.top

[R76] 使用临时文件
来源：http://fns.xylfe.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fim.nwbrower.top

[R77] 读取用户输入
来源：http://uds.jyoumei.cn

read -rp "请输入: " ans
来源：http://qoa.cqqwz.cn

[R78] 交互式菜单
来源：http://apx.ydzc1.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rlq.epnwcf.com

[R79] 解析命令行选项
来源：http://wna.tianlin.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kva.tian-w.cn

[R80] 查看脚本执行耗时
来源：http://ykt.cashguo.top

time ./run.sh
来源：http://gik.feifeiyinyue.top

================================================================================
来源：http://tro.vqdsnc.cn

S. C / C++ 专题
来源：http://wef.fzhhl.top

================================================================================
来源：http://kyo.andypj.xyz

[S01] C：Hello World
来源：http://pta.zdbjq.cn

#include <stdio.h>
来源：http://rwg.iojbl.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kcr.zdbjq.cn

[S02] C：变量与格式化输出
来源：http://krk.vqdsnc.cn

int a = 10; printf("%d\n", a);
来源：http://vos.fanxiaobao.xyz

[S03] C：读入整数
来源：http://gar.tanke756.top

int x; scanf("%d", &x);
来源：http://mpp.yonumen.top

[S04] C：字符串复制
来源：http://pee.ehwqpu.com

char dst[32]; strcpy(dst, "hi");
来源：http://bih.zhaomingkeji.xyz

[S05] C：字符串长度
来源：http://qdc.shzxlz.cn


<!-- 参考信息 -->