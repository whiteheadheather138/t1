代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://rbu.chenjidiqi.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uhq.52xcode.cn

[Q39] 自连接（查上下级）
来源：http://izv.tian-w.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://mns.zhengqikj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qtr.epnwcf.com

[Q40] 交叉连接（笛卡尔积）
来源：http://tuf.havefunace.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oym.gzhubu.top

[Q41] 多表连接
来源：http://wnn.quarkkingdee.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://nek.ybcxt.top

JOIN users u ON u.id = o.user_id
来源：http://wam.shzxlz.cn

JOIN products p ON p.id = o.product_id;
来源：http://ien.fktsv.cn

[Q42] 连接条件附加过滤
来源：http://rqz.aizwys.cn

SELECT u.name, o.amount FROM users u
来源：http://tgu.jqgufenzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cad.xuanzx.com

[Q43] 标量子查询
来源：http://cyy.0kj1m.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://swn.yfazqb.com

[Q44] IN 子查询
来源：http://dub.shuidangran.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yyu.yj20258888.top

[Q45] EXISTS 判断存在
来源：http://lpp.xingfuxueyuan.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://api.nwbrower.top

[Q46] NOT EXISTS 判断不存在
来源：http://bpk.shangyingyoupin.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bxj.meibo888.top

[Q47] 与平均值比较
来源：http://yad.tian-w.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sgx.jiagoushi.top

[Q48] CTE 公用表表达式
来源：http://qob.ehwqpu.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mhs.bjfxy.top

SELECT * FROM t WHERE c > 5;
来源：http://clh.andypj.xyz

[Q49] 更新单行
来源：http://hur.ctjpmb.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zgv.daxiang520.top

[Q50] 批量更新
来源：http://aln.ydjk.org.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pbi.iojbl.cn

[Q51] 用子查询更新
来源：http://tcu.yongpay.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xuj.shanyushiyangkeji.top

[Q52] 删除指定行
来源：http://efc.cheryme.top

DELETE FROM users WHERE id = 10;
来源：http://mpv.cheryme.top

[Q53] 按条件删除
来源：http://lrw.redwolf501.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vzo.xylfe.cn

[Q54] 清空表
来源：http://hgu.cashguo.top

TRUNCATE TABLE logs;
来源：http://pxg.havefunace.top

[Q55] 排名（并列占位）
来源：http://qnj.sweek.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yxc.yfazqb.com

[Q56] 密集排名（并列不占位）
来源：http://bru.shuidangran.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kqb.fengsongda.top

[Q57] 行号
来源：http://bjj.yuxming.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nua.hywenlv.cn

[Q58] 累计求和
来源：http://psb.c1oappe.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jrf.9152youxi.cn

[Q59] 分组内累计
来源：http://cbf.jlsjyb.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://eqn.fengsongda.top

[Q60] 取上一行 / 下一行
来源：http://wzl.sufxvd.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://isj.gotoacloud.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jrj.wangshuangyany.cn

[Q61] 移动平均
来源：http://izz.svipenyu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://aeh.iojbl.cn

[Q62] 分组占比
来源：http://lax.zycfv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gab.dianchejie.cn

[Q63] 开启事务
来源：http://tvk.ybcxt.top

START TRANSACTION;                -- 或 BEGIN
来源：http://fyx.pycfn.com

[Q64] 提交事务
来源：http://ebr.ybcxt.top

COMMIT;
来源：http://eye.yvedp.cn

[Q65] 回滚事务
来源：http://aye.cdnleiting.top

ROLLBACK;
来源：http://ypx.birdmap.top

[Q66] 行锁查询
来源：http://iwq.shanyushiyangtech.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ycv.shangyingyoupin.top

[Q67] 设置隔离级别
来源：http://fzu.jinyuanbaomall.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ukq.zhixingplan.top

[Q68] 保存点
来源：http://ske.yj202588.top

SAVEPOINT sp1;
来源：http://btu.yonumen.top

ROLLBACK TO sp1;
来源：http://tsb.xuanzx.com

[Q69] 查看执行计划
来源：http://axj.tianlin.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xqo.gotoacloud.top

[Q70] 更新统计信息
来源：http://zmc.yangfankeji.com

ANALYZE TABLE users;
来源：http://rdu.tian-w.cn

[Q71] 查看建表语句
来源：http://ipz.fzhhl.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uek.wangdashe.top

[Q72] 查看索引
来源：http://kks.vqdsnc.cn

SHOW INDEX FROM users;
来源：http://psh.fanxiaobao.xyz

[Q73] 查看表状态
来源：http://oqf.guowangkeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rad.gaohongyu789.top

[Q74] 强制使用索引
来源：http://ptm.yuxming.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lpl.ppjwa.cn

[Q75] 日期格式化
来源：http://rzp.fanxiaobao.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yek.gzhubu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jmh.gogol.net.cn

[Q76] 按天统计
来源：http://eok.svipenyu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rci.tarul.cn

[Q77] 时间加减
来源：http://pgj.hongshengwenyu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xih.jinghuilouyu.cn

[Q78] 当前时间
来源：http://erj.svipenyu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gkd.ywan-chungtsiang.top

[Q79] 字符串拼接
来源：http://vsh.fehbvm.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mkq.ydjk.org.cn

[Q80] 字符串截取
来源：http://isd.ppjwa.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://opt.jqgfzy.top

[Q81] 字符串替换
来源：http://fqc.chenjidiqi.icu

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wkd.ppjwa.cn

[Q82] 字符长度与字节长度
来源：http://hhz.ehwqpu.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zvm.dianchejie.cn

[Q83] 大小写转换
来源：http://tbj.yvedp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ote.birdmap.top

[Q84] 去除首尾空格
来源：http://vdh.ppjwa.cn

SELECT TRIM(name) FROM users;
来源：http://nnv.jinqigufen.top

[Q85] 数值取整
来源：http://pev.feifeiyinyue.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eyk.hcnkem.com

[Q86] 读取 JSON 字段
来源：http://msk.xinyue.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vat.9152youxi.cn

[Q87] JSON 字段做条件
来源：http://rim.ydzc1.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dye.uphjek.com

[Q88] 行转列（条件聚合）
来源：http://xml.zdqjudy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ouu.tanke756.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://skz.yuanzhike.top

[Q89] 判断表是否存在
来源：http://pfi.jianghu66.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oqe.bbcook.cn

[Q90] 生成序号列
来源：http://qzm.yuxming.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gjj.chenjidiqi.icu

================================================================================
来源：http://bhv.guowangkeji.top

R. Bash 专题
来源：http://aub.yvedp.cn

================================================================================
来源：http://rxx.shanyushiyangtech.top

[R01] shebang 与严格模式
来源：http://qnl.gogol.net.cn

#!/usr/bin/env bash
来源：http://kvv.yvedp.cn

set -euo pipefail
来源：http://fwp.0kj1m.cn

[R02] 变量赋值与使用
来源：http://axl.sysykeji.top

name="Tom"; echo "$name"
来源：http://amq.zdqjudy.top

[R03] 只读变量
来源：http://rwy.hcnkem.com

readonly PI=3.14
来源：http://hlp.quarkkingdee.top

[R04] 位置参数
来源：http://yns.bbcook.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gwa.zhiwuduotai.top

[R05] 参数默认值
来源：http://lyv.gaohongyu789.top

name="${1:-default}"
来源：http://xnf.ctjpmb.com

[R06] 判断命令是否存在
来源：http://fls.yuxming.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hqo.wangdashe.top

[R07] if 判断文件
来源：http://esr.jinqigfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kgx.zhiwuduotai.top

[R08] 数值比较
来源：http://nvu.ydjk.org.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rkv.quarkkingdee.top

[R09] 字符串比较
来源：http://inm.yangfankeji.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cao.sweek.top

[R10] 正则匹配
来源：http://fyw.sweek.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://emk.chenjidiqi.icu

[R11] case 多分支
来源：http://uml.haohaochexian.top

case "$1" in
来源：http://ibc.haohaochexian.top

start) echo "启动" ;;
来源：http://uyq.zhongyouzk.top

stop)  echo "停止" ;;
来源：http://ekv.shanyushiyangtech.top

*)     echo "未知命令" ;;
来源：http://wrl.0kj1m.cn

esac
来源：http://tai.hywenlv.cn

[R12] for 遍历文件
来源：http://vkm.fehbvm.com

for f in *.txt; do echo "$f"; done
来源：http://qja.fanxiaobao.xyz

[R13] for 计数循环
来源：http://agm.hfpthk.cn

for i in {1..10}; do echo "$i"; done
来源：http://ldf.jqgufenzy.top

[R14] C 风格 for
来源：http://ijx.xylfe.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://urf.xuetiantiany.cn

[R15] while 逐行读文件
来源：http://fqo.jiagoushi.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yqf.ydzc1.top

[R16] until 等待条件
来源：http://gao.vehdjk.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ycd.zhengqikj.top

[R17] 数组定义与取值
来源：http://qmc.cheryme.top

arr=(a b c); echo "${arr[0]}"
来源：http://nyw.hysaishi.cn

[R18] 遍历数组
来源：http://oqa.316326.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hmk.svipenyu.cn

[R19] 数组长度
来源：http://mwe.dashuyun.cn

echo "${#arr[@]}"
来源：http://hsx.vqdsnc.cn

[R20] 关联数组（字典）
来源：http://ueu.yonumen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tob.daxiang520.top

[R21] 字符串长度
来源：http://fna.jyoumei.cn

echo "${#s}"
来源：http://ihr.pengpengdd.cyou

[R22] 截取子串
来源：http://bcd.hywenlv.cn

echo "${s:0:5}"
来源：http://ccb.gaohongyu789.top

[R23] 字符串替换
来源：http://dwd.zhaomingkeji.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cjb.mhx1999.top

[R24] 大小写转换
来源：http://qux.9152youxi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wsa.316326.xyz

[R25] 去后缀 / 去前缀
来源：http://uis.shuidangran.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://yad.havefunace.top

[R26] 命令替换
来源：http://afs.birdmap.top

now=$(date +%F); echo "$now"
来源：http://tvk.shuidangran.top

[R27] 算术展开
来源：http://cec.xylfe.cn

echo $((1 + 2 * 3))
来源：http://jxz.hnqzz.top

[R28] 浮点运算
来源：http://gxd.zhijiandao.cn

echo "scale=2; 10/3" | bc
来源：http://aze.zhengqikj.top

[R29] 定义函数
来源：http://ekq.pengpengdd.cyou

add() { echo $(($1 + $2)); }; add 1 2
来源：http://swh.yongpay.top

[R30] 函数返回状态码
来源：http://jxl.yuxming.cn

f() { return 0; }; f || echo "失败了"
来源：http://uoi.shanyushiyangtech.top

[R31] 局部变量
来源：http://fty.sweek.top

f() { local x=1; echo "$x"; }
来源：http://lmr.iojbl.cn

[R32] 参数个数校验
来源：http://haw.chenlongwang.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rjg.zhijiandao.cn

[R33] 捕获错误并提示行号
来源：http://uhw.fzhhl.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wqj.jianghu66.top

[R34] 退出时清理
来源：http://hzm.meibo888.top

trap 'rm -f "$tmp"' EXIT
来源：http://uyb.chenlongwang.top

[R35] 后台执行并等待
来源：http://cxx.haohaochexian.top

sleep 5 & pid=$!; wait "$pid"
来源：http://gic.tianlin.xyz

[R36] 并发执行多个任务
来源：http://qvw.feifeiyinyue.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hay.zhoulong.xyz

[R37] 把输出赋给变量
来源：http://diy.hcnkem.com

files=$(ls -1)
来源：http://bup.jinyuanbaomall.cn

[R38] 管道串联
来源：http://bsr.316326.xyz

cat a.txt | grep -i error | wc -l
来源：http://zdr.mhx1999.top

[R39] 重定向标准输出与错误
来源：http://zkz.dashuyun.cn

cmd > out.log 2>&1
来源：http://vio.snrcjt.cn

[R40] 追加写日志
来源：http://twj.sjlbkw.cn

echo "log" >> out.log
来源：http://qyw.hywenlv.cn

[R41] 丢弃输出
来源：http://rwm.cheryme.top

cmd >/dev/null 2>&1
来源：http://sav.hammf.cn

[R42] 输入重定向
来源：http://ihp.pengpengdd.cyou

wc -l < a.txt
来源：http://ruj.vqdsnc.cn

[R43] 按名字查找文件
来源：http://pdx.gotoacloud.top

find . -name "*.log" -type f
来源：http://hif.hysaishi.cn

[R44] 按修改时间查找
来源：http://wwp.fktsv.cn

find . -mtime -7 -type f
来源：http://rbx.xingfuxueyuan.xyz

[R45] 批量删除
来源：http://yod.zhongyouzk.top

find . -name "*.tmp" -delete
来源：http://ane.svipenyu.cn

[R46] 递归替换文件内容
来源：http://xsp.yanxiufei.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ode.iojbl.cn

[R47] sed 单行替换
来源：http://klc.jinqigufen.top

sed -i 's/foo/bar/g' a.txt
来源：http://nkq.zdqjudy.top

[R48] awk 取指定列
来源：http://ysd.jyoumei.cn

awk '{print $1, $3}' a.txt
来源：http://vgy.zdqjudy.top

[R49] awk 带条件
来源：http://uvg.ydzc1.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wzq.shzxlz.cn

[R50] awk 求和
来源：http://afr.cashguo.top

awk '{s += $2} END {print s}' a.txt
来源：http://wmu.redwolf501.top

[R51] 排序去重取前几
来源：http://wwa.tarul.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vgm.c1oappe.top

[R52] 统计行数
来源：http://yaj.gogol.net.cn

wc -l a.txt
来源：http://fsc.hfpthk.cn

[R53] 查看文件头与实时尾
来源：http://ipl.hesvh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xwi.mhx1999.top

[R54] 比较两个文件
来源：http://ddd.zdqjudy.top

diff a.txt b.txt
来源：http://cqk.jinyuanbaomall.cn

[R55] 压缩与解压
来源：http://rnm.snrcjt.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://znt.yfazqb.com

[R56] 远程拷贝
来源：http://pld.shuidangran.top

scp file user@host:/path/
来源：http://zsr.smart0.xyz

[R57] 远程执行命令
来源：http://yrg.chenzaomai.com

ssh user@host 'uptime'
来源：http://vfw.daxiang520.top

[R58] 下载文件
来源：http://dzu.xziqi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ygf.jlsjyb.cn

[R59] 发 POST JSON
来源：http://cga.tian-w.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nbj.yj20258.top

[R60] 只看 HTTP 状态码
来源：http://dmt.hcnkem.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lcq.52xcode.cn

[R61] 磁盘占用
来源：http://xuf.pycfn.com

df -h;  du -sh *
来源：http://dfn.daxiang520.top

[R62] 找最占空间的文件
来源：http://zox.hnqzz.top

du -ah . | sort -rh | head -10
来源：http://tga.9152youxi.cn

[R63] 内存与进程
来源：http://azd.gogol.net.cn

free -h;  ps aux | grep nginx
来源：http://ayy.epnwcf.com

[R64] 结束进程
来源：http://dvf.epnwcf.com

kill -9 $(pgrep -f app.py)
来源：http://rmr.uphjek.com

[R65] 查看端口占用
来源：http://zwh.jqgufenzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zma.smart0.xyz

[R66] 定时任务
来源：http://sgm.jinyuanbaomall.cn

crontab -e;  crontab -l
来源：http://owh.gzhubu.top

[R67] 生成随机十六进制串
来源：http://wxf.gaohongyu789.top

openssl rand -hex 16
来源：http://fks.hcnkem.com

[R68] 计算文件校验值
来源：http://sin.shangyingyoupin.top

sha256sum a.txt;  md5sum a.txt
来源：http://zvr.wangshuangyany.cn

[R69] 生成随机密码
来源：http://ptn.yj20258.top

head -c 16 /dev/urandom | base64
来源：http://xfq.tianlin.xyz

[R70] 时间戳与互转
来源：http://osz.smart0.xyz

date +%s;  date -d @1700000000
来源：http://toi.cucudq.cn

[R71] 日期格式化
来源：http://ftu.xingfuxueyuan.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://rwu.guowangkeji.top

[R72] 等待端口就绪
来源：http://oog.jyoumei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://awj.sysykeji.top

[R73] 分割大日志
来源：http://rmf.hnxiangtu.top

split -l 1000 big.log part_
来源：http://bbu.ivvv.top

[R74] 批量重命名
来源：http://fnd.ydzc1.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://aai.zhengqikj.top

[R75] 导出环境变量
来源：http://txd.tarul.cn

export PATH="$HOME/bin:$PATH"
来源：http://pgb.xuanzx.com

[R76] 使用临时文件
来源：http://gpw.yanxiufei.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pcp.smart0.xyz

[R77] 读取用户输入
来源：http://kel.sweek.top

read -rp "请输入: " ans
来源：http://lhb.havefunace.top

[R78] 交互式菜单
来源：http://qog.zhoulong.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://oyp.birdmap.top

[R79] 解析命令行选项
来源：http://tqd.gaohongyu789.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://aoe.bjfxy.top

[R80] 查看脚本执行耗时
来源：http://wfu.fktsv.cn

time ./run.sh
来源：http://wrs.jqgfzy.top

================================================================================
来源：http://ilw.xingfuxueyuan.xyz

S. C / C++ 专题
来源：http://raz.yj202588.top

================================================================================
来源：http://bfw.fktsv.cn

[S01] C：Hello World
来源：http://yrm.wangdashe.top

#include <stdio.h>
来源：http://jne.guowangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://brc.jinqigfzy.top

[S02] C：变量与格式化输出
来源：http://baz.gaohongyu789.top

int a = 10; printf("%d\n", a);
来源：http://qxq.zhiwuduotai.top

[S03] C：读入整数
来源：http://mfm.hywenlv.cn

int x; scanf("%d", &x);
来源：http://yoc.zhijiandao.cn

[S04] C：字符串复制
来源：http://dge.yuanzhike.top

char dst[32]; strcpy(dst, "hi");
来源：http://jwi.yj20258888.top

[S05] C：字符串长度
来源：http://zjh.gogol.net.cn

strlen(s)
来源：http://jjp.ybcxt.top

[S06] C：字符串比较
来源：http://wot.sxryk.cn

strcmp(a, b) == 0
来源：http://ljg.cucudq.cn

[S07] C：数组遍历求和
来源：http://axr.c1oappe.top


<!-- 参考信息 -->