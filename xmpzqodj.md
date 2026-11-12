代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://him.316326.xyz

JOIN users u ON u.id = o.user_id
来源：http://kuy.316326.xyz

JOIN products p ON p.id = o.product_id;
来源：http://oce.nanxinkj.top

[Q42] 连接条件附加过滤
来源：http://ewi.9152youxi.cn

SELECT u.name, o.amount FROM users u
来源：http://kcw.jiagoushi.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qod.shanyushiyangkeji.top

[Q43] 标量子查询
来源：http://ucy.dashuyun.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://csm.nanxuanxn.top

[Q44] IN 子查询
来源：http://idv.shzxlz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ona.redwolf501.top

[Q45] EXISTS 判断存在
来源：http://opv.tianlin.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pzu.xziqi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xpm.epnwcf.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rqz.daria6918.cn

[Q47] 与平均值比较
来源：http://abv.zhixingplan.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jau.zhaomingkeji.xyz

[Q48] CTE 公用表表达式
来源：http://phs.shzxlz.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mwo.xuanzx.com

SELECT * FROM t WHERE c > 5;
来源：http://azo.hesvh.cn

[Q49] 更新单行
来源：http://fce.andypj.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mue.yj20258888.top

[Q50] 批量更新
来源：http://ihr.cdnleiting.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vrj.nwbrower.top

[Q51] 用子查询更新
来源：http://xen.jiagoushi.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mpi.chenjidiqi.icu

[Q52] 删除指定行
来源：http://jpm.jinghuilouyu.cn

DELETE FROM users WHERE id = 10;
来源：http://jph.jinqigfzy.top

[Q53] 按条件删除
来源：http://syd.hfpthk.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cnr.haohaochexian.top

[Q54] 清空表
来源：http://byk.jiagoushi.top

TRUNCATE TABLE logs;
来源：http://jhb.ydzc1.top

[Q55] 排名（并列占位）
来源：http://jbx.mhx1999.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vcb.yj20258.top

[Q56] 密集排名（并列不占位）
来源：http://zvc.hywenlv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oig.andypj.xyz

[Q57] 行号
来源：http://pxf.ywan-chungtsiang.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uhx.xziqi.cn

[Q58] 累计求和
来源：http://cfj.yj202588.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ywk.chenlongwang.top

[Q59] 分组内累计
来源：http://arr.cucudq.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://def.guannengcc.top

[Q60] 取上一行 / 下一行
来源：http://moi.jqgufenzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qnr.gzhubu.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yig.c1oappe.top

[Q61] 移动平均
来源：http://clk.guannengcc.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wts.jiagoushi.top

[Q62] 分组占比
来源：http://xli.tianlin.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rii.xinyue.icu

[Q63] 开启事务
来源：http://nst.cdnleiting.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dxq.cqqwz.cn

[Q64] 提交事务
来源：http://ssz.epnwcf.com

COMMIT;
来源：http://apw.fehbvm.com

[Q65] 回滚事务
来源：http://ggr.hammf.cn

ROLLBACK;
来源：http://iqc.quarkkingdee.top

[Q66] 行锁查询
来源：http://akm.iojbl.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pic.9152youxi.cn

[Q67] 设置隔离级别
来源：http://oeq.zhengqikj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qit.hnqzz.top

[Q68] 保存点
来源：http://ebl.feifeiyinyue.top

SAVEPOINT sp1;
来源：http://ovk.jqgufenzy.top

ROLLBACK TO sp1;
来源：http://zjj.gogol.net.cn

[Q69] 查看执行计划
来源：http://wpq.hongshengwenyu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vft.nwbrower.top

[Q70] 更新统计信息
来源：http://hfu.chenzaomai.com

ANALYZE TABLE users;
来源：http://iqp.feifeiyinyue.top

[Q71] 查看建表语句
来源：http://pgn.ehwqpu.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lis.redwolf501.top

[Q72] 查看索引
来源：http://rsd.sysykeji.top

SHOW INDEX FROM users;
来源：http://igh.hnqzz.top

[Q73] 查看表状态
来源：http://fgy.shangyingyoupin.top

SHOW TABLE STATUS LIKE 'users';
来源：http://zwz.52xcode.cn

[Q74] 强制使用索引
来源：http://lov.gotoacloud.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mwc.cashguo.top

[Q75] 日期格式化
来源：http://pvd.wangdashe.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sxw.fktsv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yzy.cdnleiting.top

[Q76] 按天统计
来源：http://tzr.zdbjq.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lcd.uphjek.com

[Q77] 时间加减
来源：http://jih.fehbvm.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jtw.sweek.top

[Q78] 当前时间
来源：http://ill.bbcook.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zsv.jiagoushi.top

[Q79] 字符串拼接
来源：http://loh.zhongyouzk.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lve.tarul.cn

[Q80] 字符串截取
来源：http://tgb.hongshengwenyu.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://khd.fktsv.cn

[Q81] 字符串替换
来源：http://sxv.ydzc1.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hwz.gaohongyu789.top

[Q82] 字符长度与字节长度
来源：http://hla.yj20258.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://som.yanxiufei.cn

[Q83] 大小写转换
来源：http://dzy.chenlongwang.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fnr.aibaodan.cn

[Q84] 去除首尾空格
来源：http://nkz.yueranfly.top

SELECT TRIM(name) FROM users;
来源：http://kqb.yangfankeji.com

[Q85] 数值取整
来源：http://acg.jyoumei.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bsp.gogol.net.cn

[Q86] 读取 JSON 字段
来源：http://pqi.yangfankeji.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lzl.sxryk.cn

[Q87] JSON 字段做条件
来源：http://tnf.fzhhl.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jll.316326.xyz

[Q88] 行转列（条件聚合）
来源：http://hno.redwolf501.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jsl.hfpthk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://syo.nanxuanxn.top

[Q89] 判断表是否存在
来源：http://rbb.xziqi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xhc.zdbjq.cn

[Q90] 生成序号列
来源：http://cbz.sweek.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nbv.xuetiantiany.cn

================================================================================
来源：http://gpk.xylfe.cn

R. Bash 专题
来源：http://vii.fanxiaobao.xyz

================================================================================
来源：http://fcu.hnxiangtu.top

[R01] shebang 与严格模式
来源：http://usb.yueranfly.top

#!/usr/bin/env bash
来源：http://ssn.svipenyu.cn

set -euo pipefail
来源：http://hwj.cqqwz.cn

[R02] 变量赋值与使用
来源：http://xat.daxiang520.top

name="Tom"; echo "$name"
来源：http://apg.daria6918.cn

[R03] 只读变量
来源：http://gwg.gotoacloud.top

readonly PI=3.14
来源：http://frv.hcnkem.com

[R04] 位置参数
来源：http://yku.hcnkem.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sxu.gzhubu.top

[R05] 参数默认值
来源：http://tjk.jinyuanbaomall.cn

name="${1:-default}"
来源：http://vkj.guowangkeji.top

[R06] 判断命令是否存在
来源：http://ypy.ywan-chungtsiang.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gpb.fktsv.cn

[R07] if 判断文件
来源：http://bis.jinqigfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kva.shanyushiyangtech.top

[R08] 数值比较
来源：http://olh.sjlbkw.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cga.iojbl.cn

[R09] 字符串比较
来源：http://psj.sjlbkw.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wkh.jiagoushi.top

[R10] 正则匹配
来源：http://rbp.aibaodan.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mnu.dianchejie.cn

[R11] case 多分支
来源：http://cgl.yfazqb.com

case "$1" in
来源：http://hmj.fzhhl.top

start) echo "启动" ;;
来源：http://vwj.shanyushiyangtech.top

stop)  echo "停止" ;;
来源：http://zfo.zhijiandao.cn

*)     echo "未知命令" ;;
来源：http://aqi.316326.xyz

esac
来源：http://vbu.yfazqb.com

[R12] for 遍历文件
来源：http://ljs.hywenlv.cn

for f in *.txt; do echo "$f"; done
来源：http://omd.bjfxy.top

[R13] for 计数循环
来源：http://bhw.haohaochexian.top

for i in {1..10}; do echo "$i"; done
来源：http://cms.chenjidiqi.icu

[R14] C 风格 for
来源：http://npr.daria6918.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qqs.ywan-chungtsiang.top

[R15] while 逐行读文件
来源：http://uxk.wangdashe.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uig.yongpay.top

[R16] until 等待条件
来源：http://pfy.birdmap.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kzr.wangshuangyany.cn

[R17] 数组定义与取值
来源：http://eca.nanxinkj.top

arr=(a b c); echo "${arr[0]}"
来源：http://krz.epnwcf.com

[R18] 遍历数组
来源：http://xil.zhoulong.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jva.havefunace.top

[R19] 数组长度
来源：http://zsd.ehwqpu.com

echo "${#arr[@]}"
来源：http://gcw.fengsongda.top

[R20] 关联数组（字典）
来源：http://utp.yuxming.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yvd.andypj.xyz

[R21] 字符串长度
来源：http://ssa.aibaodan.cn

echo "${#s}"
来源：http://cfy.ybcxt.top

[R22] 截取子串
来源：http://xdy.jiagoushi.top

echo "${s:0:5}"
来源：http://xro.cucudq.cn

[R23] 字符串替换
来源：http://ont.quarkkingdee.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vee.cqqwz.cn

[R24] 大小写转换
来源：http://fjt.feifeiyinyue.top

echo "${s^^}"; echo "${s,,}"
来源：http://roe.pengpengdd.cyou

[R25] 去后缀 / 去前缀
来源：http://ojl.yanxiufei.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://htf.zhongyouzk.top

[R26] 命令替换
来源：http://mfq.zhiwuduotai.top

now=$(date +%F); echo "$now"
来源：http://aqj.guannengcc.top

[R27] 算术展开
来源：http://hhv.tanke756.top

echo $((1 + 2 * 3))
来源：http://vov.ppjwa.cn

[R28] 浮点运算
来源：http://cgi.xziqi.cn

echo "scale=2; 10/3" | bc
来源：http://gks.hysaishi.cn

[R29] 定义函数
来源：http://bde.vqdsnc.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qnw.hnxiangtu.top

[R30] 函数返回状态码
来源：http://pgz.guannengcc.top

f() { return 0; }; f || echo "失败了"
来源：http://gdg.feifeiyinyue.top

[R31] 局部变量
来源：http://lbz.ehwqpu.com

f() { local x=1; echo "$x"; }
来源：http://vqu.fzhhl.top

[R32] 参数个数校验
来源：http://ser.gotoacloud.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ytq.nwbrower.top

[R33] 捕获错误并提示行号
来源：http://iyq.zhongyouzk.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fwu.xziqi.cn

[R34] 退出时清理
来源：http://ras.zhongyouzk.top

trap 'rm -f "$tmp"' EXIT
来源：http://bee.cdnleiting.top

[R35] 后台执行并等待
来源：http://tiw.shuidangran.top

sleep 5 & pid=$!; wait "$pid"
来源：http://tfq.gogol.net.cn

[R36] 并发执行多个任务
来源：http://qtp.shzxlz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wuk.hnxiangtu.top

[R37] 把输出赋给变量
来源：http://etj.cashguo.top

files=$(ls -1)
来源：http://aoo.birdmap.top

[R38] 管道串联
来源：http://rji.ybcxt.top

cat a.txt | grep -i error | wc -l
来源：http://ezt.cheryme.top

[R39] 重定向标准输出与错误
来源：http://fqt.fehbvm.com

cmd > out.log 2>&1
来源：http://rfw.wangshuangyany.cn

[R40] 追加写日志
来源：http://yfb.ydzc1.top

echo "log" >> out.log
来源：http://fnz.quarkkingdee.top

[R41] 丢弃输出
来源：http://qxc.wangshuangyany.cn

cmd >/dev/null 2>&1
来源：http://pga.havefunace.top

[R42] 输入重定向
来源：http://qfy.havefunace.top

wc -l < a.txt
来源：http://pmi.hammf.cn

[R43] 按名字查找文件
来源：http://jgm.xziqi.cn

find . -name "*.log" -type f
来源：http://kau.zhixingplan.top

[R44] 按修改时间查找
来源：http://ywy.hysaishi.cn

find . -mtime -7 -type f
来源：http://rug.shzxlz.cn

[R45] 批量删除
来源：http://mwd.bjfxy.top

find . -name "*.tmp" -delete
来源：http://qss.zhengqikj.top

[R46] 递归替换文件内容
来源：http://wam.shanyushiyangtech.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mpy.sweek.top

[R47] sed 单行替换
来源：http://gpu.jinghuilouyu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zsc.shzxlz.cn

[R48] awk 取指定列
来源：http://ffl.yueranfly.top

awk '{print $1, $3}' a.txt
来源：http://bff.chenzaomai.com

[R49] awk 带条件
来源：http://cwg.shangyingyoupin.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vle.fehbvm.com

[R50] awk 求和
来源：http://mlo.jlsjyb.cn

awk '{s += $2} END {print s}' a.txt
来源：http://khp.hammf.cn

[R51] 排序去重取前几
来源：http://pvj.vehdjk.com

sort a.txt | uniq -c | sort -rn | head
来源：http://frq.quarkkingdee.top

[R52] 统计行数
来源：http://ndj.chenjidiqi.icu

wc -l a.txt
来源：http://lec.guannengcc.top

[R53] 查看文件头与实时尾
来源：http://jqx.yj20258.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zah.jianghu66.top

[R54] 比较两个文件
来源：http://wbp.sysykeji.top

diff a.txt b.txt
来源：http://nem.vehdjk.com

[R55] 压缩与解压
来源：http://eye.jyoumei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jcs.haohaochexian.top

[R56] 远程拷贝
来源：http://wmz.zhengqikj.top

scp file user@host:/path/
来源：http://nbg.yuxming.cn

[R57] 远程执行命令
来源：http://yon.fzhhl.top

ssh user@host 'uptime'
来源：http://ron.chenlongwang.top

[R58] 下载文件
来源：http://tzk.shanyushiyangtech.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://poo.snrcjt.cn

[R59] 发 POST JSON
来源：http://wkc.guannengcc.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gwu.yj202588.top

[R60] 只看 HTTP 状态码
来源：http://fzi.yj20258888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://aqt.hnqzz.top

[R61] 磁盘占用
来源：http://gde.hnxiangtu.top

df -h;  du -sh *
来源：http://htt.ppjwa.cn

[R62] 找最占空间的文件
来源：http://bwg.dashuyun.cn

du -ah . | sort -rh | head -10
来源：http://fwg.meibo888.top

[R63] 内存与进程
来源：http://idg.sysykeji.top

free -h;  ps aux | grep nginx
来源：http://ygu.zhaomingkeji.xyz

[R64] 结束进程
来源：http://vvr.zhaomingkeji.xyz

kill -9 $(pgrep -f app.py)
来源：http://vnl.dashuyun.cn

[R65] 查看端口占用
来源：http://qvq.zhoulong.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kcn.cashguo.top

[R66] 定时任务
来源：http://iis.bjfxy.top

crontab -e;  crontab -l
来源：http://fwp.shangyingyoupin.top

[R67] 生成随机十六进制串
来源：http://qpc.andypj.xyz

openssl rand -hex 16
来源：http://zqp.xuanzx.com

[R68] 计算文件校验值
来源：http://les.yj20258888.top

sha256sum a.txt;  md5sum a.txt
来源：http://gof.vqdsnc.cn

[R69] 生成随机密码
来源：http://eng.nanxinkj.top

head -c 16 /dev/urandom | base64
来源：http://vde.ppjwa.cn

[R70] 时间戳与互转
来源：http://sky.zhoulong.xyz

date +%s;  date -d @1700000000
来源：http://ybt.daxiang520.top

[R71] 日期格式化
来源：http://wix.ydjk.org.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://aaw.uphjek.com

[R72] 等待端口就绪
来源：http://sim.snrcjt.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ngb.dianchejie.cn

[R73] 分割大日志
来源：http://aqw.yj202588.top

split -l 1000 big.log part_
来源：http://adj.haohaochexian.top

[R74] 批量重命名
来源：http://gmr.jlsjyb.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vpy.pengpengdd.cyou

[R75] 导出环境变量
来源：http://rub.yuanzhike.top

export PATH="$HOME/bin:$PATH"
来源：http://ghr.yangfankeji.com

[R76] 使用临时文件
来源：http://tvl.gzhubu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://oqo.ppjwa.cn

[R77] 读取用户输入
来源：http://xui.bjfxy.top

read -rp "请输入: " ans
来源：http://eyu.52xcode.cn

[R78] 交互式菜单
来源：http://drr.yuxming.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zld.epnwcf.com

[R79] 解析命令行选项
来源：http://nij.fktsv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ppt.52xcode.cn

[R80] 查看脚本执行耗时
来源：http://qfn.cdnleiting.top

time ./run.sh
来源：http://znx.birdmap.top

================================================================================
来源：http://eip.snrcjt.cn

S. C / C++ 专题
来源：http://hxo.zhijiandao.cn

================================================================================
来源：http://nzm.wangdashe.top

[S01] C：Hello World
来源：http://xtm.shuidangran.top

#include <stdio.h>
来源：http://std.cashguo.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://pen.tian-w.cn

[S02] C：变量与格式化输出
来源：http://byx.zdqjudy.top

int a = 10; printf("%d\n", a);
来源：http://htn.52xcode.cn

[S03] C：读入整数
来源：http://kne.dianchejie.cn

int x; scanf("%d", &x);
来源：http://wvc.havefunace.top

[S04] C：字符串复制
来源：http://lsm.ehwqpu.com

char dst[32]; strcpy(dst, "hi");
来源：http://rxt.xinyue.icu

[S05] C：字符串长度
来源：http://aeq.jqgufenzy.top

strlen(s)
来源：http://zko.cheryme.top

[S06] C：字符串比较
来源：http://hqb.andypj.xyz

strcmp(a, b) == 0
来源：http://koc.gogol.net.cn

[S07] C：数组遍历求和
来源：http://qqd.andypj.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hqe.yj20258.top

[S08] C：动态内存分配与释放
来源：http://uzt.zhaomingkeji.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://czn.bbcook.cn

[S09] C：结构体定义与初始化
来源：http://rwe.yj20258888.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hvb.shuidangran.top

[S10] C：指针与解引用
来源：http://ois.ehwqpu.com

int *p = &a;  *p = 5;
来源：http://wsd.yvedp.cn

[S11] C：逐行读文件
来源：http://cjx.cqqwz.cn


<!-- 参考信息 -->