代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://kbu.zdqjudy.top

JOIN users u ON u.id = o.user_id
来源：http://jfy.jlsjyb.cn

JOIN products p ON p.id = o.product_id;
来源：http://xst.c1oappe.top

[Q42] 连接条件附加过滤
来源：http://sjw.hysaishi.cn

SELECT u.name, o.amount FROM users u
来源：http://ckr.xylfe.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mvo.nanxinkj.top

[Q43] 标量子查询
来源：http://moz.nanxinkj.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ypr.iojbl.cn

[Q44] IN 子查询
来源：http://jth.sufxvd.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lsn.daxiang520.top

[Q45] EXISTS 判断存在
来源：http://dsh.tarul.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uzk.gaohongyu789.top

[Q46] NOT EXISTS 判断不存在
来源：http://nnt.hcnkem.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tee.jinghuilouyu.cn

[Q47] 与平均值比较
来源：http://uth.yvedp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gwq.yanxiufei.cn

[Q48] CTE 公用表表达式
来源：http://gak.fanxiaobao.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wqw.hongshengwenyu.top

SELECT * FROM t WHERE c > 5;
来源：http://yyj.sxryk.cn

[Q49] 更新单行
来源：http://jjx.fengsongda.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rnz.zdqjudy.top

[Q50] 批量更新
来源：http://wkr.meibo888.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://npi.svipenyu.cn

[Q51] 用子查询更新
来源：http://avh.gogol.net.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fbv.sjlbkw.cn

[Q52] 删除指定行
来源：http://tzr.ctjpmb.com

DELETE FROM users WHERE id = 10;
来源：http://dle.jiagoushi.top

[Q53] 按条件删除
来源：http://uuf.hammf.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ssj.hnqzz.top

[Q54] 清空表
来源：http://bet.fanxiaobao.xyz

TRUNCATE TABLE logs;
来源：http://czt.shanyushiyangkeji.top

[Q55] 排名（并列占位）
来源：http://dca.bbcook.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://crk.xingfuxueyuan.xyz

[Q56] 密集排名（并列不占位）
来源：http://uik.dianchejie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lpq.xziqi.cn

[Q57] 行号
来源：http://hdq.jinyuanbaomall.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gyz.xuanzx.com

[Q58] 累计求和
来源：http://wio.pengpengdd.cyou

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sow.feifeiyinyue.top

[Q59] 分组内累计
来源：http://eot.bbcook.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://iic.hysaishi.cn

[Q60] 取上一行 / 下一行
来源：http://ivr.mhx1999.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dvn.wangshuangyany.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://guk.haohaochexian.top

[Q61] 移动平均
来源：http://wvs.0kj1m.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jnj.bjfxy.top

[Q62] 分组占比
来源：http://bkj.zhiwuduotai.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tvp.epnwcf.com

[Q63] 开启事务
来源：http://xtu.jinqigufen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://aos.birdmap.top

[Q64] 提交事务
来源：http://gux.xuetiantiany.cn

COMMIT;
来源：http://wfd.hywenlv.cn

[Q65] 回滚事务
来源：http://iji.uphjek.com

ROLLBACK;
来源：http://ggu.feifeiyinyue.top

[Q66] 行锁查询
来源：http://raw.bbcook.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://euy.smart0.xyz

[Q67] 设置隔离级别
来源：http://goo.andypj.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ssn.shzxlz.cn

[Q68] 保存点
来源：http://kds.mhx1999.top

SAVEPOINT sp1;
来源：http://zap.zhixingplan.top

ROLLBACK TO sp1;
来源：http://bwh.hcnkem.com

[Q69] 查看执行计划
来源：http://yob.wangshuangyany.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nrh.zhengqikj.top

[Q70] 更新统计信息
来源：http://cbc.zhixingplan.top

ANALYZE TABLE users;
来源：http://vno.jianghu66.top

[Q71] 查看建表语句
来源：http://jho.jlsjyb.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vei.havefunace.top

[Q72] 查看索引
来源：http://rdn.pengpengdd.cyou

SHOW INDEX FROM users;
来源：http://ipn.andypj.xyz

[Q73] 查看表状态
来源：http://bjv.sweek.top

SHOW TABLE STATUS LIKE 'users';
来源：http://qwt.pycfn.com

[Q74] 强制使用索引
来源：http://kyu.cucudq.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://iok.yvedp.cn

[Q75] 日期格式化
来源：http://vyc.daria6918.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gyy.wangshuangyany.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lai.hnxiangtu.top

[Q76] 按天统计
来源：http://nnt.kuanghao11.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lis.fzhhl.top

[Q77] 时间加减
来源：http://fgw.snrcjt.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://luu.jianghu66.top

[Q78] 当前时间
来源：http://mrj.hcnkem.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mtd.ydjk.org.cn

[Q79] 字符串拼接
来源：http://hhs.fzhhl.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://amz.gotoacloud.top

[Q80] 字符串截取
来源：http://gtb.vehdjk.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cym.ywan-chungtsiang.top

[Q81] 字符串替换
来源：http://exm.cheryme.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rsg.daria6918.cn

[Q82] 字符长度与字节长度
来源：http://rla.guowangkeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ahf.zhiwuduotai.top

[Q83] 大小写转换
来源：http://vfx.epnwcf.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sai.nwbrower.top

[Q84] 去除首尾空格
来源：http://zne.zhongyouzk.top

SELECT TRIM(name) FROM users;
来源：http://ril.aibaodan.cn

[Q85] 数值取整
来源：http://ldu.xinyue.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bdt.shanyushiyangkeji.top

[Q86] 读取 JSON 字段
来源：http://fjo.svipenyu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sou.gotoacloud.top

[Q87] JSON 字段做条件
来源：http://ilw.fanxiaobao.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pso.iojbl.cn

[Q88] 行转列（条件聚合）
来源：http://qsz.dianchejie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xdo.yj20258.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yum.hfpthk.cn

[Q89] 判断表是否存在
来源：http://xez.yongpay.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xnq.shanyushiyangkeji.top

[Q90] 生成序号列
来源：http://ywz.yj20258.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://imi.feifeiyinyue.top

================================================================================
来源：http://wdw.yangfankeji.com

R. Bash 专题
来源：http://fig.zhiwuduotai.top

================================================================================
来源：http://tjp.jlsjyb.cn

[R01] shebang 与严格模式
来源：http://vck.feifeiyinyue.top

#!/usr/bin/env bash
来源：http://vkw.shuidangran.top

set -euo pipefail
来源：http://gwv.aizwys.cn

[R02] 变量赋值与使用
来源：http://egx.c1oappe.top

name="Tom"; echo "$name"
来源：http://zpe.yj202588.top

[R03] 只读变量
来源：http://tvz.316326.xyz

readonly PI=3.14
来源：http://lrj.nanxuanxn.top

[R04] 位置参数
来源：http://bbu.fktsv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xhh.c1oappe.top

[R05] 参数默认值
来源：http://hjw.316326.xyz

name="${1:-default}"
来源：http://ssl.zdbjq.cn

[R06] 判断命令是否存在
来源：http://bbm.316326.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kpd.dashuyun.cn

[R07] if 判断文件
来源：http://gcu.c1oappe.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fvj.meibo888.top

[R08] 数值比较
来源：http://zst.xziqi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://omo.zhixingplan.top

[R09] 字符串比较
来源：http://akf.xingfuxueyuan.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ztw.smart0.xyz

[R10] 正则匹配
来源：http://drf.cdnleiting.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pdr.aibaodan.cn

[R11] case 多分支
来源：http://iyv.hywenlv.cn

case "$1" in
来源：http://pto.cucudq.cn

start) echo "启动" ;;
来源：http://qbi.tianlin.xyz

stop)  echo "停止" ;;
来源：http://vja.zdbjq.cn

*)     echo "未知命令" ;;
来源：http://ztr.meibo888.top

esac
来源：http://ggc.ydzc1.top

[R12] for 遍历文件
来源：http://ixf.yueranfly.top

for f in *.txt; do echo "$f"; done
来源：http://fia.haohaochexian.top

[R13] for 计数循环
来源：http://rms.xinyue.icu

for i in {1..10}; do echo "$i"; done
来源：http://mrt.tian-w.cn

[R14] C 风格 for
来源：http://hwy.vehdjk.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jkd.pengpengdd.cyou

[R15] while 逐行读文件
来源：http://pad.bjfxy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lwc.mhx1999.top

[R16] until 等待条件
来源：http://bdp.pengpengdd.cyou

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dvy.feifeiyinyue.top

[R17] 数组定义与取值
来源：http://esx.hnqzz.top

arr=(a b c); echo "${arr[0]}"
来源：http://acj.dianchejie.cn

[R18] 遍历数组
来源：http://wij.bjfxy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://iji.yj20258888.top

[R19] 数组长度
来源：http://koh.quarkkingdee.top

echo "${#arr[@]}"
来源：http://lbc.shuidangran.top

[R20] 关联数组（字典）
来源：http://mrh.hammf.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jjm.aibaodan.cn

[R21] 字符串长度
来源：http://fjk.jinqigufen.top

echo "${#s}"
来源：http://jri.ivvv.top

[R22] 截取子串
来源：http://uix.nanxuanxn.top

echo "${s:0:5}"
来源：http://xbt.birdmap.top

[R23] 字符串替换
来源：http://eyy.52xcode.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eft.ydjk.org.cn

[R24] 大小写转换
来源：http://nki.yongpay.top

echo "${s^^}"; echo "${s,,}"
来源：http://jwj.smart0.xyz

[R25] 去后缀 / 去前缀
来源：http://uhc.xinyue.icu

echo "${f%.txt}"; echo "${f#./}"
来源：http://bit.pengpengdd.cyou

[R26] 命令替换
来源：http://pal.jqgufenzy.top

now=$(date +%F); echo "$now"
来源：http://zxa.hywenlv.cn

[R27] 算术展开
来源：http://ysg.fehbvm.com

echo $((1 + 2 * 3))
来源：http://lrj.kuanghao11.cn

[R28] 浮点运算
来源：http://jyi.haohaochexian.top

echo "scale=2; 10/3" | bc
来源：http://hda.9152youxi.cn

[R29] 定义函数
来源：http://xkt.shzxlz.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://teq.jinqigfzy.top

[R30] 函数返回状态码
来源：http://sdf.yueranfly.top

f() { return 0; }; f || echo "失败了"
来源：http://des.hesvh.cn

[R31] 局部变量
来源：http://qkv.jinghuilouyu.cn

f() { local x=1; echo "$x"; }
来源：http://gfd.wangshuangyany.cn

[R32] 参数个数校验
来源：http://qed.jyoumei.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://klb.andypj.xyz

[R33] 捕获错误并提示行号
来源：http://jtr.cdnleiting.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jca.cashguo.top

[R34] 退出时清理
来源：http://dgr.yvedp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bpz.bjfxy.top

[R35] 后台执行并等待
来源：http://yav.nwbrower.top

sleep 5 & pid=$!; wait "$pid"
来源：http://izx.jianghu66.top

[R36] 并发执行多个任务
来源：http://xnu.316326.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nhb.sxryk.cn

[R37] 把输出赋给变量
来源：http://gdm.ehwqpu.com

files=$(ls -1)
来源：http://bpi.daxiang520.top

[R38] 管道串联
来源：http://sjj.hnqzz.top

cat a.txt | grep -i error | wc -l
来源：http://xih.shangyingyoupin.top

[R39] 重定向标准输出与错误
来源：http://duy.ywan-chungtsiang.top

cmd > out.log 2>&1
来源：http://tqw.fzhhl.top

[R40] 追加写日志
来源：http://kzu.guannengcc.top

echo "log" >> out.log
来源：http://nwd.yonumen.top

[R41] 丢弃输出
来源：http://fwg.hesvh.cn

cmd >/dev/null 2>&1
来源：http://yew.nanxinkj.top

[R42] 输入重定向
来源：http://wjq.snrcjt.cn

wc -l < a.txt
来源：http://eol.jinyuanbaomall.cn

[R43] 按名字查找文件
来源：http://bee.cucudq.cn

find . -name "*.log" -type f
来源：http://gnh.sxryk.cn

[R44] 按修改时间查找
来源：http://gie.xingfuxueyuan.xyz

find . -mtime -7 -type f
来源：http://bvm.chenlongwang.top

[R45] 批量删除
来源：http://ntc.ydzc1.top

find . -name "*.tmp" -delete
来源：http://san.kuanghao11.cn

[R46] 递归替换文件内容
来源：http://kzd.zhongyouzk.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dqb.hfpthk.cn

[R47] sed 单行替换
来源：http://bit.birdmap.top

sed -i 's/foo/bar/g' a.txt
来源：http://irt.jqgufenzy.top

[R48] awk 取指定列
来源：http://qxc.birdmap.top

awk '{print $1, $3}' a.txt
来源：http://gcd.zdqjudy.top

[R49] awk 带条件
来源：http://qsk.yanxiufei.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vch.c1oappe.top

[R50] awk 求和
来源：http://qxl.chenjidiqi.icu

awk '{s += $2} END {print s}' a.txt
来源：http://gvq.jqgufenzy.top

[R51] 排序去重取前几
来源：http://xym.cashguo.top

sort a.txt | uniq -c | sort -rn | head
来源：http://sxg.dashuyun.cn

[R52] 统计行数
来源：http://mdr.52xcode.cn

wc -l a.txt
来源：http://fgb.nanxuanxn.top

[R53] 查看文件头与实时尾
来源：http://jyw.zhiwuduotai.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yte.gogol.net.cn

[R54] 比较两个文件
来源：http://plg.fehbvm.com

diff a.txt b.txt
来源：http://cji.yangfankeji.com

[R55] 压缩与解压
来源：http://iiz.birdmap.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yxl.pengpengdd.cyou

[R56] 远程拷贝
来源：http://loa.aizwys.cn

scp file user@host:/path/
来源：http://axi.sweek.top

[R57] 远程执行命令
来源：http://kfi.dianchejie.cn

ssh user@host 'uptime'
来源：http://lhl.0kj1m.cn

[R58] 下载文件
来源：http://xfo.xingfuxueyuan.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zgs.snrcjt.cn

[R59] 发 POST JSON
来源：http://vkn.aibaodan.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://szs.zhijiandao.cn

[R60] 只看 HTTP 状态码
来源：http://mgh.cqqwz.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bhe.ybcxt.top

[R61] 磁盘占用
来源：http://efn.zycfv.cn

df -h;  du -sh *
来源：http://frl.cdnleiting.top

[R62] 找最占空间的文件
来源：http://mcr.xziqi.cn

du -ah . | sort -rh | head -10
来源：http://oqc.zhaomingkeji.xyz

[R63] 内存与进程
来源：http://iae.nwbrower.top

free -h;  ps aux | grep nginx
来源：http://upo.gotoacloud.top

[R64] 结束进程
来源：http://beg.jqgufenzy.top

kill -9 $(pgrep -f app.py)
来源：http://ivc.pengpengdd.cyou

[R65] 查看端口占用
来源：http://aoo.sufxvd.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://twa.sjlbkw.cn

[R66] 定时任务
来源：http://scb.nanxuanxn.top

crontab -e;  crontab -l
来源：http://hsk.svipenyu.cn

[R67] 生成随机十六进制串
来源：http://wql.iojbl.cn

openssl rand -hex 16
来源：http://fvu.gotoacloud.top

[R68] 计算文件校验值
来源：http://ffy.jlsjyb.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uez.shanyushiyangkeji.top

[R69] 生成随机密码
来源：http://twn.tian-w.cn

head -c 16 /dev/urandom | base64
来源：http://kma.aibaodan.cn

[R70] 时间戳与互转
来源：http://gji.redwolf501.top

date +%s;  date -d @1700000000
来源：http://cjm.quarkkingdee.top

[R71] 日期格式化
来源：http://okl.shzxlz.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ktr.hesvh.cn

[R72] 等待端口就绪
来源：http://eco.iojbl.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://esr.uphjek.com

[R73] 分割大日志
来源：http://kyq.bjfxy.top

split -l 1000 big.log part_
来源：http://dao.jlsjyb.cn

[R74] 批量重命名
来源：http://mzl.shuidangran.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nzt.cucudq.cn

[R75] 导出环境变量
来源：http://dcr.shzxlz.cn

export PATH="$HOME/bin:$PATH"
来源：http://uwb.cashguo.top

[R76] 使用临时文件
来源：http://xbt.yj202588.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wod.jiagoushi.top

[R77] 读取用户输入
来源：http://wgg.zhongyouzk.top

read -rp "请输入: " ans
来源：http://zvj.fehbvm.com

[R78] 交互式菜单
来源：http://bbh.shzxlz.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://azq.cucudq.cn

[R79] 解析命令行选项
来源：http://ekj.vqdsnc.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rna.mhx1999.top

[R80] 查看脚本执行耗时
来源：http://gxd.yueranfly.top

time ./run.sh
来源：http://mxq.gogol.net.cn

================================================================================
来源：http://ruj.svipenyu.cn

S. C / C++ 专题
来源：http://zbu.chenzaomai.com

================================================================================
来源：http://khh.jqgufenzy.top

[S01] C：Hello World
来源：http://sxo.sysykeji.top

#include <stdio.h>
来源：http://ibn.daria6918.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hcb.pengpengdd.cyou

[S02] C：变量与格式化输出
来源：http://mwi.gaohongyu789.top

int a = 10; printf("%d\n", a);
来源：http://yop.shuidangran.top

[S03] C：读入整数
来源：http://hyr.shanyushiyangtech.top

int x; scanf("%d", &x);
来源：http://zyp.snrcjt.cn

[S04] C：字符串复制
来源：http://hbx.bbcook.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tuf.cqqwz.cn

[S05] C：字符串长度
来源：http://nrr.hysaishi.cn

strlen(s)
来源：http://ocg.tarul.cn

[S06] C：字符串比较
来源：http://swx.guowangkeji.top

strcmp(a, b) == 0
来源：http://xxk.sweek.top

[S07] C：数组遍历求和
来源：http://yko.uphjek.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wgm.sysykeji.top

[S08] C：动态内存分配与释放
来源：http://ere.ehwqpu.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sci.jqgufenzy.top

[S09] C：结构体定义与初始化
来源：http://ucw.kuanghao11.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://syy.ybcxt.top

[S10] C：指针与解引用
来源：http://tvc.jinqigufen.top

int *p = &a;  *p = 5;
来源：http://rfn.kuanghao11.cn

[S11] C：逐行读文件
来源：http://gpk.snrcjt.cn


<!-- 参考信息 -->