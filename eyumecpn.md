代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://grr.shzxlz.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ohp.c1oappe.top

[Q39] 自连接（查上下级）
来源：http://sqp.ppjwa.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kbv.hysaishi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://amv.zhongyouzk.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zpf.hcnkem.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wfu.shuidangran.top

[Q41] 多表连接
来源：http://gih.bjfxy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://qcw.ehwqpu.com

JOIN users u ON u.id = o.user_id
来源：http://nvi.yj202588.top

JOIN products p ON p.id = o.product_id;
来源：http://zqi.ppjwa.cn

[Q42] 连接条件附加过滤
来源：http://gcc.aibaodan.cn

SELECT u.name, o.amount FROM users u
来源：http://mib.nwbrower.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nla.tanke756.top

[Q43] 标量子查询
来源：http://frj.hesvh.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yzm.zhixingplan.top

[Q44] IN 子查询
来源：http://egs.xylfe.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lld.havefunace.top

[Q45] EXISTS 判断存在
来源：http://tnp.tianlin.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eyo.chenzaomai.com

[Q46] NOT EXISTS 判断不存在
来源：http://dcv.cdnleiting.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ksk.zhijiandao.cn

[Q47] 与平均值比较
来源：http://oed.yuanzhike.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qzq.yj20258.top

[Q48] CTE 公用表表达式
来源：http://xnu.sxryk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rck.gzhubu.top

SELECT * FROM t WHERE c > 5;
来源：http://jwo.gotoacloud.top

[Q49] 更新单行
来源：http://qyb.bbcook.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fvc.xziqi.cn

[Q50] 批量更新
来源：http://uov.jinyuanbaomall.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://awx.yanxiufei.cn

[Q51] 用子查询更新
来源：http://wcg.bjfxy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ukp.kuanghao11.cn

[Q52] 删除指定行
来源：http://ycm.sjlbkw.cn

DELETE FROM users WHERE id = 10;
来源：http://auu.shzxlz.cn

[Q53] 按条件删除
来源：http://sjv.sjlbkw.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://goh.hnqzz.top

[Q54] 清空表
来源：http://xpp.fktsv.cn

TRUNCATE TABLE logs;
来源：http://umv.sweek.top

[Q55] 排名（并列占位）
来源：http://dgl.jinyuanbaomall.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dnk.fengsongda.top

[Q56] 密集排名（并列不占位）
来源：http://asz.316326.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kdh.zhijiandao.cn

[Q57] 行号
来源：http://prf.quarkkingdee.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tol.bjfxy.top

[Q58] 累计求和
来源：http://bnk.fzhhl.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://oer.52xcode.cn

[Q59] 分组内累计
来源：http://aar.chenjidiqi.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qug.andypj.xyz

[Q60] 取上一行 / 下一行
来源：http://lae.gotoacloud.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://aaq.smart0.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cio.hywenlv.cn

[Q61] 移动平均
来源：http://nsx.uphjek.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bpi.havefunace.top

[Q62] 分组占比
来源：http://krg.vqdsnc.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vsk.tian-w.cn

[Q63] 开启事务
来源：http://ehh.feifeiyinyue.top

START TRANSACTION;                -- 或 BEGIN
来源：http://woh.ivvv.top

[Q64] 提交事务
来源：http://wmz.fanxiaobao.xyz

COMMIT;
来源：http://hhu.jqgufenzy.top

[Q65] 回滚事务
来源：http://dpk.sjlbkw.cn

ROLLBACK;
来源：http://mme.sysykeji.top

[Q66] 行锁查询
来源：http://ryt.fehbvm.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ltp.xuanzx.com

[Q67] 设置隔离级别
来源：http://rtw.yonumen.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bxw.jyoumei.cn

[Q68] 保存点
来源：http://frf.zycfv.cn

SAVEPOINT sp1;
来源：http://ebf.vqdsnc.cn

ROLLBACK TO sp1;
来源：http://dps.havefunace.top

[Q69] 查看执行计划
来源：http://qyo.fanxiaobao.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tmn.shanyushiyangkeji.top

[Q70] 更新统计信息
来源：http://qgw.wangshuangyany.cn

ANALYZE TABLE users;
来源：http://cyv.mhx1999.top

[Q71] 查看建表语句
来源：http://ibg.yj20258.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://riw.xingfuxueyuan.xyz

[Q72] 查看索引
来源：http://pvp.0kj1m.cn

SHOW INDEX FROM users;
来源：http://pgm.yvedp.cn

[Q73] 查看表状态
来源：http://suz.nwbrower.top

SHOW TABLE STATUS LIKE 'users';
来源：http://xkh.yangfankeji.com

[Q74] 强制使用索引
来源：http://qol.birdmap.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fhv.vehdjk.com

[Q75] 日期格式化
来源：http://zef.hysaishi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nuk.sysykeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://job.jqgfzy.top

[Q76] 按天统计
来源：http://mgq.shanyushiyangkeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rpd.jinyuanbaomall.cn

[Q77] 时间加减
来源：http://mvj.tian-w.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zeo.jinyuanbaomall.cn

[Q78] 当前时间
来源：http://inw.chenjidiqi.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jhk.shzxlz.cn

[Q79] 字符串拼接
来源：http://udw.sysykeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iie.yueranfly.top

[Q80] 字符串截取
来源：http://bxk.zycfv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fgv.epnwcf.com

[Q81] 字符串替换
来源：http://ofq.pycfn.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hhf.sysykeji.top

[Q82] 字符长度与字节长度
来源：http://cwu.316326.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hxg.zdbjq.cn

[Q83] 大小写转换
来源：http://vca.redwolf501.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cjq.xuanzx.com

[Q84] 去除首尾空格
来源：http://jus.zhengqikj.top

SELECT TRIM(name) FROM users;
来源：http://hft.tarul.cn

[Q85] 数值取整
来源：http://mkg.zhaomingkeji.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mza.nanxinkj.top

[Q86] 读取 JSON 字段
来源：http://bkb.jqgufenzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://azo.yanxiufei.cn

[Q87] JSON 字段做条件
来源：http://ndv.xziqi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lfq.hfpthk.cn

[Q88] 行转列（条件聚合）
来源：http://byx.9152youxi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ruz.ydjk.org.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lsv.sysykeji.top

[Q89] 判断表是否存在
来源：http://pgs.wangshuangyany.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gkf.bbcook.cn

[Q90] 生成序号列
来源：http://ehk.jyoumei.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xjj.xinyue.icu

================================================================================
来源：http://uoc.ppjwa.cn

R. Bash 专题
来源：http://tjx.zhaomingkeji.xyz

================================================================================
来源：http://vra.chenzaomai.com

[R01] shebang 与严格模式
来源：http://sxc.kuanghao11.cn

#!/usr/bin/env bash
来源：http://lea.jinyuanbaomall.cn

set -euo pipefail
来源：http://tyw.shanyushiyangkeji.top

[R02] 变量赋值与使用
来源：http://gas.yueranfly.top

name="Tom"; echo "$name"
来源：http://jlk.ehwqpu.com

[R03] 只读变量
来源：http://ahv.hongshengwenyu.top

readonly PI=3.14
来源：http://otm.zycfv.cn

[R04] 位置参数
来源：http://aau.ivvv.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ibl.yuanzhike.top

[R05] 参数默认值
来源：http://fvw.snrcjt.cn

name="${1:-default}"
来源：http://ate.fanxiaobao.xyz

[R06] 判断命令是否存在
来源：http://rpb.cheryme.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dwq.smart0.xyz

[R07] if 判断文件
来源：http://zwy.ydzc1.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mtj.xylfe.cn

[R08] 数值比较
来源：http://oci.52xcode.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gnw.hongshengwenyu.top

[R09] 字符串比较
来源：http://gik.xziqi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://aal.jqgufenzy.top

[R10] 正则匹配
来源：http://wvp.kuanghao11.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zzh.yanxiufei.cn

[R11] case 多分支
来源：http://zij.zhijiandao.cn

case "$1" in
来源：http://acg.iojbl.cn

start) echo "启动" ;;
来源：http://nue.haohaochexian.top

stop)  echo "停止" ;;
来源：http://pgf.ywan-chungtsiang.top

*)     echo "未知命令" ;;
来源：http://xnu.zhiwuduotai.top

esac
来源：http://nrn.epnwcf.com

[R12] for 遍历文件
来源：http://ven.zhixingplan.top

for f in *.txt; do echo "$f"; done
来源：http://vhc.xinyue.icu

[R13] for 计数循环
来源：http://caq.wangdashe.top

for i in {1..10}; do echo "$i"; done
来源：http://ewp.xuanzx.com

[R14] C 风格 for
来源：http://uoi.haohaochexian.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vnt.yfazqb.com

[R15] while 逐行读文件
来源：http://eof.hammf.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kxo.c1oappe.top

[R16] until 等待条件
来源：http://hcv.zhaomingkeji.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ojv.wangdashe.top

[R17] 数组定义与取值
来源：http://zjh.ydjk.org.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dow.sjlbkw.cn

[R18] 遍历数组
来源：http://hza.9152youxi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uho.shanyushiyangkeji.top

[R19] 数组长度
来源：http://gww.c1oappe.top

echo "${#arr[@]}"
来源：http://ibh.yj202588.top

[R20] 关联数组（字典）
来源：http://vbe.fehbvm.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uer.jianghu66.top

[R21] 字符串长度
来源：http://aic.cucudq.cn

echo "${#s}"
来源：http://rtw.yfazqb.com

[R22] 截取子串
来源：http://pek.ydzc1.top

echo "${s:0:5}"
来源：http://ovh.nanxuanxn.top

[R23] 字符串替换
来源：http://icu.gzhubu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://spw.nwbrower.top

[R24] 大小写转换
来源：http://yhw.daxiang520.top

echo "${s^^}"; echo "${s,,}"
来源：http://alh.jqgfzy.top

[R25] 去后缀 / 去前缀
来源：http://uir.jlsjyb.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kaq.hongshengwenyu.top

[R26] 命令替换
来源：http://fkd.iojbl.cn

now=$(date +%F); echo "$now"
来源：http://kro.cashguo.top

[R27] 算术展开
来源：http://okr.cashguo.top

echo $((1 + 2 * 3))
来源：http://qzm.gogol.net.cn

[R28] 浮点运算
来源：http://omr.vqdsnc.cn

echo "scale=2; 10/3" | bc
来源：http://ttz.sysykeji.top

[R29] 定义函数
来源：http://qof.meibo888.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xda.jyoumei.cn

[R30] 函数返回状态码
来源：http://hxw.zdbjq.cn

f() { return 0; }; f || echo "失败了"
来源：http://ihs.hnqzz.top

[R31] 局部变量
来源：http://nnz.ydjk.org.cn

f() { local x=1; echo "$x"; }
来源：http://fkl.zhaomingkeji.xyz

[R32] 参数个数校验
来源：http://wtz.hcnkem.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qua.shuidangran.top

[R33] 捕获错误并提示行号
来源：http://hli.haohaochexian.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rix.cdnleiting.top

[R34] 退出时清理
来源：http://myp.kuanghao11.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xvj.snrcjt.cn

[R35] 后台执行并等待
来源：http://gsq.nanxuanxn.top

sleep 5 & pid=$!; wait "$pid"
来源：http://evg.jiagoushi.top

[R36] 并发执行多个任务
来源：http://syt.ctjpmb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xok.fktsv.cn

[R37] 把输出赋给变量
来源：http://yxc.birdmap.top

files=$(ls -1)
来源：http://vym.zhengqikj.top

[R38] 管道串联
来源：http://oro.jqgufenzy.top

cat a.txt | grep -i error | wc -l
来源：http://hbz.ctjpmb.com

[R39] 重定向标准输出与错误
来源：http://hla.vehdjk.com

cmd > out.log 2>&1
来源：http://xpp.sysykeji.top

[R40] 追加写日志
来源：http://thm.dashuyun.cn

echo "log" >> out.log
来源：http://bbf.nwbrower.top

[R41] 丢弃输出
来源：http://stb.ydzc1.top

cmd >/dev/null 2>&1
来源：http://jzc.zhixingplan.top

[R42] 输入重定向
来源：http://cxg.sjlbkw.cn

wc -l < a.txt
来源：http://sdm.hesvh.cn

[R43] 按名字查找文件
来源：http://jsm.shuidangran.top

find . -name "*.log" -type f
来源：http://cjs.daria6918.cn

[R44] 按修改时间查找
来源：http://jly.sweek.top

find . -mtime -7 -type f
来源：http://anq.svipenyu.cn

[R45] 批量删除
来源：http://tiw.yfazqb.com

find . -name "*.tmp" -delete
来源：http://cxe.cashguo.top

[R46] 递归替换文件内容
来源：http://gja.feifeiyinyue.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wlt.cdnleiting.top

[R47] sed 单行替换
来源：http://uqd.hesvh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nom.xziqi.cn

[R48] awk 取指定列
来源：http://orx.gotoacloud.top

awk '{print $1, $3}' a.txt
来源：http://amb.zhengqikj.top

[R49] awk 带条件
来源：http://pvj.xuanzx.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://syt.gogol.net.cn

[R50] awk 求和
来源：http://awc.shangyingyoupin.top

awk '{s += $2} END {print s}' a.txt
来源：http://fwb.jinqigufen.top

[R51] 排序去重取前几
来源：http://yzg.52xcode.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zfz.uphjek.com

[R52] 统计行数
来源：http://ceq.nwbrower.top

wc -l a.txt
来源：http://ezw.xinyue.icu

[R53] 查看文件头与实时尾
来源：http://bbf.0kj1m.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tds.yuxming.cn

[R54] 比较两个文件
来源：http://mzj.zhaomingkeji.xyz

diff a.txt b.txt
来源：http://nxp.zhiwuduotai.top

[R55] 压缩与解压
来源：http://cxy.yj20258888.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vgf.pycfn.com

[R56] 远程拷贝
来源：http://kyl.ivvv.top

scp file user@host:/path/
来源：http://zsx.hfpthk.cn

[R57] 远程执行命令
来源：http://huh.mhx1999.top

ssh user@host 'uptime'
来源：http://cbm.gaohongyu789.top

[R58] 下载文件
来源：http://ssb.cheryme.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pua.ctjpmb.com

[R59] 发 POST JSON
来源：http://cqp.yonumen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qjw.pengpengdd.cyou

[R60] 只看 HTTP 状态码
来源：http://zmz.ppjwa.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://but.quarkkingdee.top

[R61] 磁盘占用
来源：http://bgj.bjfxy.top

df -h;  du -sh *
来源：http://obk.zdbjq.cn

[R62] 找最占空间的文件
来源：http://bjl.jyoumei.cn

du -ah . | sort -rh | head -10
来源：http://bru.cucudq.cn

[R63] 内存与进程
来源：http://suw.kuanghao11.cn

free -h;  ps aux | grep nginx
来源：http://lfg.yanxiufei.cn

[R64] 结束进程
来源：http://swx.cheryme.top

kill -9 $(pgrep -f app.py)
来源：http://eqz.guowangkeji.top

[R65] 查看端口占用
来源：http://kjw.sufxvd.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vmp.hnqzz.top

[R66] 定时任务
来源：http://mdz.zycfv.cn

crontab -e;  crontab -l
来源：http://xpf.zycfv.cn

[R67] 生成随机十六进制串
来源：http://eri.yj202588.top

openssl rand -hex 16
来源：http://zpj.redwolf501.top

[R68] 计算文件校验值
来源：http://qyc.gzhubu.top

sha256sum a.txt;  md5sum a.txt
来源：http://khj.vehdjk.com

[R69] 生成随机密码
来源：http://der.gaohongyu789.top

head -c 16 /dev/urandom | base64
来源：http://rlm.ppjwa.cn

[R70] 时间戳与互转
来源：http://kdh.ydzc1.top

date +%s;  date -d @1700000000
来源：http://gdz.zdbjq.cn

[R71] 日期格式化
来源：http://gzq.tanke756.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://gip.c1oappe.top

[R72] 等待端口就绪
来源：http://pek.smart0.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://qcm.aizwys.cn

[R73] 分割大日志
来源：http://nur.hywenlv.cn

split -l 1000 big.log part_
来源：http://cmb.0kj1m.cn

[R74] 批量重命名
来源：http://zbe.zhaomingkeji.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vfi.fehbvm.com

[R75] 导出环境变量
来源：http://lwp.tianlin.xyz

export PATH="$HOME/bin:$PATH"
来源：http://wtk.yueranfly.top

[R76] 使用临时文件
来源：http://drx.nanxinkj.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qnr.meibo888.top

[R77] 读取用户输入
来源：http://ftu.yangfankeji.com

read -rp "请输入: " ans
来源：http://mjy.zhijiandao.cn

[R78] 交互式菜单
来源：http://ggr.shangyingyoupin.top

select opt in a b c; do echo "$opt"; break; done
来源：http://bsh.gaohongyu789.top

[R79] 解析命令行选项
来源：http://bat.jyoumei.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ncx.jinyuanbaomall.cn

[R80] 查看脚本执行耗时
来源：http://qgb.yvedp.cn

time ./run.sh
来源：http://lua.316326.xyz

================================================================================
来源：http://dbu.redwolf501.top

S. C / C++ 专题
来源：http://zfz.zhiwuduotai.top

================================================================================
来源：http://jbt.hcnkem.com

[S01] C：Hello World
来源：http://rzc.epnwcf.com

#include <stdio.h>
来源：http://cay.cucudq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bjh.tarul.cn

[S02] C：变量与格式化输出
来源：http://xeq.cdnleiting.top

int a = 10; printf("%d\n", a);
来源：http://vcs.zycfv.cn

[S03] C：读入整数
来源：http://unj.fengsongda.top

int x; scanf("%d", &x);
来源：http://umx.bjfxy.top

[S04] C：字符串复制
来源：http://tae.meibo888.top

char dst[32]; strcpy(dst, "hi");
来源：http://buu.fzhhl.top

[S05] C：字符串长度
来源：http://pew.ywan-chungtsiang.top

strlen(s)
来源：http://gwd.quarkkingdee.top

[S06] C：字符串比较
来源：http://bvt.zhixingplan.top

strcmp(a, b) == 0
来源：http://inc.yvedp.cn

[S07] C：数组遍历求和
来源：http://wkw.tanke756.top


<!-- 参考信息 -->