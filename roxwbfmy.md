代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kxp.hywenlv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qhq.xylfe.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zoz.gzhubu.top

[Q41] 多表连接
来源：http://xml.fzhhl.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://uou.jlsjyb.cn

JOIN users u ON u.id = o.user_id
来源：http://cud.dianchejie.cn

JOIN products p ON p.id = o.product_id;
来源：http://jcw.yonumen.top

[Q42] 连接条件附加过滤
来源：http://ynn.snrcjt.cn

SELECT u.name, o.amount FROM users u
来源：http://kwh.xylfe.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mza.tarul.cn

[Q43] 标量子查询
来源：http://wem.andypj.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xcw.xingfuxueyuan.xyz

[Q44] IN 子查询
来源：http://bfy.quarkkingdee.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kfm.shanyushiyangkeji.top

[Q45] EXISTS 判断存在
来源：http://ybq.shangyingyoupin.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yac.hammf.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fvm.wangdashe.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tvn.hysaishi.cn

[Q47] 与平均值比较
来源：http://fin.pycfn.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bgc.quarkkingdee.top

[Q48] CTE 公用表表达式
来源：http://rdt.xylfe.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://apd.shzxlz.cn

SELECT * FROM t WHERE c > 5;
来源：http://amd.ywan-chungtsiang.top

[Q49] 更新单行
来源：http://dlj.iojbl.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kcr.sysykeji.top

[Q50] 批量更新
来源：http://uqn.shzxlz.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zem.zycfv.cn

[Q51] 用子查询更新
来源：http://gzk.yvedp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://urh.zhaomingkeji.xyz

[Q52] 删除指定行
来源：http://kyw.nanxinkj.top

DELETE FROM users WHERE id = 10;
来源：http://bse.xziqi.cn

[Q53] 按条件删除
来源：http://ytm.hammf.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dok.feifeiyinyue.top

[Q54] 清空表
来源：http://qlm.sysykeji.top

TRUNCATE TABLE logs;
来源：http://wvd.chenjidiqi.icu

[Q55] 排名（并列占位）
来源：http://bpr.ywan-chungtsiang.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ahc.havefunace.top

[Q56] 密集排名（并列不占位）
来源：http://sdt.tianlin.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rxb.yangfankeji.com

[Q57] 行号
来源：http://uxz.jqgufenzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://spq.jqgufenzy.top

[Q58] 累计求和
来源：http://nic.xylfe.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qri.yuanzhike.top

[Q59] 分组内累计
来源：http://oda.hfpthk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kft.smart0.xyz

[Q60] 取上一行 / 下一行
来源：http://ems.kuanghao11.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bhd.52xcode.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bdk.havefunace.top

[Q61] 移动平均
来源：http://atp.cucudq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pve.sxryk.cn

[Q62] 分组占比
来源：http://lki.yanxiufei.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zbv.kuanghao11.cn

[Q63] 开启事务
来源：http://cru.c1oappe.top

START TRANSACTION;                -- 或 BEGIN
来源：http://znb.jyoumei.cn

[Q64] 提交事务
来源：http://cnz.hcnkem.com

COMMIT;
来源：http://jdx.chenjidiqi.icu

[Q65] 回滚事务
来源：http://zaj.smart0.xyz

ROLLBACK;
来源：http://jow.sxryk.cn

[Q66] 行锁查询
来源：http://ozd.ybcxt.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xte.aizwys.cn

[Q67] 设置隔离级别
来源：http://gup.gogol.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zfw.jinyuanbaomall.cn

[Q68] 保存点
来源：http://qey.yj20258.top

SAVEPOINT sp1;
来源：http://ula.daria6918.cn

ROLLBACK TO sp1;
来源：http://wyj.gogol.net.cn

[Q69] 查看执行计划
来源：http://kns.jlsjyb.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rag.nanxinkj.top

[Q70] 更新统计信息
来源：http://bxf.andypj.xyz

ANALYZE TABLE users;
来源：http://zrh.redwolf501.top

[Q71] 查看建表语句
来源：http://wip.xingfuxueyuan.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://psj.kuanghao11.cn

[Q72] 查看索引
来源：http://eri.wangshuangyany.cn

SHOW INDEX FROM users;
来源：http://lsc.uphjek.com

[Q73] 查看表状态
来源：http://oll.ydzc1.top

SHOW TABLE STATUS LIKE 'users';
来源：http://kdj.shangyingyoupin.top

[Q74] 强制使用索引
来源：http://nwa.xziqi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hrv.jianghu66.top

[Q75] 日期格式化
来源：http://uhk.jinqigufen.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jra.yanxiufei.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://iqr.zhoulong.xyz

[Q76] 按天统计
来源：http://bon.shuidangran.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rch.vehdjk.com

[Q77] 时间加减
来源：http://nbj.jinghuilouyu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zkx.mhx1999.top

[Q78] 当前时间
来源：http://xdy.hywenlv.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://icv.gotoacloud.top

[Q79] 字符串拼接
来源：http://qkq.zhongyouzk.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mlv.birdmap.top

[Q80] 字符串截取
来源：http://kbd.zdbjq.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fjb.316326.xyz

[Q81] 字符串替换
来源：http://jcy.pycfn.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gug.gotoacloud.top

[Q82] 字符长度与字节长度
来源：http://xkz.zhengqikj.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rev.zhixingplan.top

[Q83] 大小写转换
来源：http://gnn.xuetiantiany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://iuq.shangyingyoupin.top

[Q84] 去除首尾空格
来源：http://isd.hammf.cn

SELECT TRIM(name) FROM users;
来源：http://csn.zhengqikj.top

[Q85] 数值取整
来源：http://qor.feifeiyinyue.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lua.cdnleiting.top

[Q86] 读取 JSON 字段
来源：http://uoh.sysykeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tuy.hcnkem.com

[Q87] JSON 字段做条件
来源：http://lwj.fehbvm.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://grl.ywan-chungtsiang.top

[Q88] 行转列（条件聚合）
来源：http://sal.snrcjt.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wkp.xinyue.icu

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ruq.aizwys.cn

[Q89] 判断表是否存在
来源：http://fwn.cucudq.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pxz.yvedp.cn

[Q90] 生成序号列
来源：http://hfo.zhongyouzk.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rsv.fehbvm.com

================================================================================
来源：http://eri.hnxiangtu.top

R. Bash 专题
来源：http://enh.mhx1999.top

================================================================================
来源：http://qle.hfpthk.cn

[R01] shebang 与严格模式
来源：http://kou.pycfn.com

#!/usr/bin/env bash
来源：http://rbz.daria6918.cn

set -euo pipefail
来源：http://abd.jlsjyb.cn

[R02] 变量赋值与使用
来源：http://rec.hcnkem.com

name="Tom"; echo "$name"
来源：http://sfx.havefunace.top

[R03] 只读变量
来源：http://zox.zhongyouzk.top

readonly PI=3.14
来源：http://exb.pengpengdd.cyou

[R04] 位置参数
来源：http://pel.birdmap.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mpn.xinyue.icu

[R05] 参数默认值
来源：http://zms.hammf.cn

name="${1:-default}"
来源：http://wtu.jlsjyb.cn

[R06] 判断命令是否存在
来源：http://rkp.hammf.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://alr.52xcode.cn

[R07] if 判断文件
来源：http://cfe.quarkkingdee.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://euz.yonumen.top

[R08] 数值比较
来源：http://fdk.fzhhl.top

if (( a > b )); then echo "a 更大"; fi
来源：http://bim.epnwcf.com

[R09] 字符串比较
来源：http://exn.epnwcf.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://the.c1oappe.top

[R10] 正则匹配
来源：http://vfi.ctjpmb.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ivg.zhongyouzk.top

[R11] case 多分支
来源：http://srm.sxryk.cn

case "$1" in
来源：http://qwa.daria6918.cn

start) echo "启动" ;;
来源：http://eyo.zhixingplan.top

stop)  echo "停止" ;;
来源：http://clp.tarul.cn

*)     echo "未知命令" ;;
来源：http://zhv.yj202588.top

esac
来源：http://hsq.hcnkem.com

[R12] for 遍历文件
来源：http://jkw.tanke756.top

for f in *.txt; do echo "$f"; done
来源：http://fbv.daria6918.cn

[R13] for 计数循环
来源：http://hir.xinyue.icu

for i in {1..10}; do echo "$i"; done
来源：http://pna.gogol.net.cn

[R14] C 风格 for
来源：http://twi.9152youxi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://drl.sufxvd.cn

[R15] while 逐行读文件
来源：http://bcd.snrcjt.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mlr.iojbl.cn

[R16] until 等待条件
来源：http://ybn.hfpthk.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sln.fehbvm.com

[R17] 数组定义与取值
来源：http://zuj.xylfe.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oac.yj20258888.top

[R18] 遍历数组
来源：http://iro.nanxuanxn.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jty.jlsjyb.cn

[R19] 数组长度
来源：http://gfh.jinyuanbaomall.cn

echo "${#arr[@]}"
来源：http://qoi.iojbl.cn

[R20] 关联数组（字典）
来源：http://kna.yanxiufei.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fcl.zhaomingkeji.xyz

[R21] 字符串长度
来源：http://dqf.zhengqikj.top

echo "${#s}"
来源：http://nwh.shzxlz.cn

[R22] 截取子串
来源：http://vbh.yuxming.cn

echo "${s:0:5}"
来源：http://jzp.andypj.xyz

[R23] 字符串替换
来源：http://qts.fzhhl.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://arw.316326.xyz

[R24] 大小写转换
来源：http://mpa.aibaodan.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zmd.yvedp.cn

[R25] 去后缀 / 去前缀
来源：http://stp.zdbjq.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ali.ydjk.org.cn

[R26] 命令替换
来源：http://tkw.shuidangran.top

now=$(date +%F); echo "$now"
来源：http://cay.iojbl.cn

[R27] 算术展开
来源：http://zxy.aibaodan.cn

echo $((1 + 2 * 3))
来源：http://nob.haohaochexian.top

[R28] 浮点运算
来源：http://bwo.zhixingplan.top

echo "scale=2; 10/3" | bc
来源：http://mld.ybcxt.top

[R29] 定义函数
来源：http://sxe.yonumen.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ept.tanke756.top

[R30] 函数返回状态码
来源：http://vzj.yj20258.top

f() { return 0; }; f || echo "失败了"
来源：http://jec.yvedp.cn

[R31] 局部变量
来源：http://rps.birdmap.top

f() { local x=1; echo "$x"; }
来源：http://rkv.yj20258888.top

[R32] 参数个数校验
来源：http://srs.zhaomingkeji.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://caw.zdbjq.cn

[R33] 捕获错误并提示行号
来源：http://fke.shangyingyoupin.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lox.wangshuangyany.cn

[R34] 退出时清理
来源：http://qzs.gzhubu.top

trap 'rm -f "$tmp"' EXIT
来源：http://qcm.yj202588.top

[R35] 后台执行并等待
来源：http://xoh.xuetiantiany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cts.nanxuanxn.top

[R36] 并发执行多个任务
来源：http://wju.gzhubu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://azn.yvedp.cn

[R37] 把输出赋给变量
来源：http://zue.yongpay.top

files=$(ls -1)
来源：http://dpn.hywenlv.cn

[R38] 管道串联
来源：http://mya.pengpengdd.cyou

cat a.txt | grep -i error | wc -l
来源：http://xfs.zdbjq.cn

[R39] 重定向标准输出与错误
来源：http://dfm.cqqwz.cn

cmd > out.log 2>&1
来源：http://ekn.bjfxy.top

[R40] 追加写日志
来源：http://xmz.uphjek.com

echo "log" >> out.log
来源：http://wxa.gzhubu.top

[R41] 丢弃输出
来源：http://jio.smart0.xyz

cmd >/dev/null 2>&1
来源：http://rhx.jlsjyb.cn

[R42] 输入重定向
来源：http://dob.hesvh.cn

wc -l < a.txt
来源：http://kpr.nwbrower.top

[R43] 按名字查找文件
来源：http://waa.cashguo.top

find . -name "*.log" -type f
来源：http://arh.sufxvd.cn

[R44] 按修改时间查找
来源：http://yin.jqgfzy.top

find . -mtime -7 -type f
来源：http://ysk.gotoacloud.top

[R45] 批量删除
来源：http://zyd.feifeiyinyue.top

find . -name "*.tmp" -delete
来源：http://dff.ehwqpu.com

[R46] 递归替换文件内容
来源：http://xgg.xuanzx.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yrs.vehdjk.com

[R47] sed 单行替换
来源：http://qjl.52xcode.cn

sed -i 's/foo/bar/g' a.txt
来源：http://oby.zhengqikj.top

[R48] awk 取指定列
来源：http://pln.haohaochexian.top

awk '{print $1, $3}' a.txt
来源：http://aqx.9152youxi.cn

[R49] awk 带条件
来源：http://qqp.sysykeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dgr.xuetiantiany.cn

[R50] awk 求和
来源：http://itc.guannengcc.top

awk '{s += $2} END {print s}' a.txt
来源：http://zfr.zhiwuduotai.top

[R51] 排序去重取前几
来源：http://jkm.jqgufenzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://obp.cucudq.cn

[R52] 统计行数
来源：http://viy.nanxuanxn.top

wc -l a.txt
来源：http://qeh.dashuyun.cn

[R53] 查看文件头与实时尾
来源：http://ukm.kuanghao11.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://arx.wangshuangyany.cn

[R54] 比较两个文件
来源：http://bhe.nanxinkj.top

diff a.txt b.txt
来源：http://csq.quarkkingdee.top

[R55] 压缩与解压
来源：http://hah.nanxuanxn.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jfz.ppjwa.cn

[R56] 远程拷贝
来源：http://fpd.hfpthk.cn

scp file user@host:/path/
来源：http://esp.redwolf501.top

[R57] 远程执行命令
来源：http://imi.yuanzhike.top

ssh user@host 'uptime'
来源：http://mjy.gzhubu.top

[R58] 下载文件
来源：http://kcc.zhijiandao.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ibx.sysykeji.top

[R59] 发 POST JSON
来源：http://pzl.ydjk.org.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gly.jinyuanbaomall.cn

[R60] 只看 HTTP 状态码
来源：http://kek.hywenlv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ytq.cdnleiting.top

[R61] 磁盘占用
来源：http://xov.ybcxt.top

df -h;  du -sh *
来源：http://qey.vqdsnc.cn

[R62] 找最占空间的文件
来源：http://uzb.cucudq.cn

du -ah . | sort -rh | head -10
来源：http://iwj.bbcook.cn

[R63] 内存与进程
来源：http://kze.yanxiufei.cn

free -h;  ps aux | grep nginx
来源：http://uzz.birdmap.top

[R64] 结束进程
来源：http://cyw.zhoulong.xyz

kill -9 $(pgrep -f app.py)
来源：http://igb.ppjwa.cn

[R65] 查看端口占用
来源：http://bxg.wangdashe.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://iqa.epnwcf.com

[R66] 定时任务
来源：http://dcl.haohaochexian.top

crontab -e;  crontab -l
来源：http://kql.hnxiangtu.top

[R67] 生成随机十六进制串
来源：http://oyp.tianlin.xyz

openssl rand -hex 16
来源：http://vyz.cqqwz.cn

[R68] 计算文件校验值
来源：http://eaf.fanxiaobao.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://wzq.jqgufenzy.top

[R69] 生成随机密码
来源：http://hin.zhaomingkeji.xyz

head -c 16 /dev/urandom | base64
来源：http://pos.yfazqb.com

[R70] 时间戳与互转
来源：http://tfx.shzxlz.cn

date +%s;  date -d @1700000000
来源：http://kzr.uphjek.com

[R71] 日期格式化
来源：http://gea.yueranfly.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://wuk.guannengcc.top

[R72] 等待端口就绪
来源：http://jhn.cqqwz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xzi.zhoulong.xyz

[R73] 分割大日志
来源：http://bkf.52xcode.cn

split -l 1000 big.log part_
来源：http://hfc.epnwcf.com

[R74] 批量重命名
来源：http://vcj.fktsv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kqn.jinghuilouyu.cn

[R75] 导出环境变量
来源：http://pnc.haohaochexian.top

export PATH="$HOME/bin:$PATH"
来源：http://jdz.jinghuilouyu.cn

[R76] 使用临时文件
来源：http://sxm.ppjwa.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://juh.zhixingplan.top

[R77] 读取用户输入
来源：http://ctf.epnwcf.com

read -rp "请输入: " ans
来源：http://eui.hnxiangtu.top

[R78] 交互式菜单
来源：http://ome.birdmap.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hmx.mhx1999.top

[R79] 解析命令行选项
来源：http://hiq.ywan-chungtsiang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hkz.vqdsnc.cn

[R80] 查看脚本执行耗时
来源：http://dww.yuanzhike.top

time ./run.sh
来源：http://jfr.feifeiyinyue.top

================================================================================
来源：http://pag.dianchejie.cn

S. C / C++ 专题
来源：http://cqm.zhijiandao.cn

================================================================================
来源：http://wve.pengpengdd.cyou

[S01] C：Hello World
来源：http://eqz.shuidangran.top

#include <stdio.h>
来源：http://ikr.gotoacloud.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://thj.guowangkeji.top

[S02] C：变量与格式化输出
来源：http://qnr.cucudq.cn

int a = 10; printf("%d\n", a);
来源：http://dye.fengsongda.top

[S03] C：读入整数
来源：http://ipk.aizwys.cn

int x; scanf("%d", &x);
来源：http://hqc.bbcook.cn

[S04] C：字符串复制
来源：http://kbe.zdqjudy.top

char dst[32]; strcpy(dst, "hi");
来源：http://ukt.ydjk.org.cn

[S05] C：字符串长度
来源：http://mvy.chenlongwang.top

strlen(s)
来源：http://rzh.hnxiangtu.top

[S06] C：字符串比较
来源：http://dxh.yj20258.top

strcmp(a, b) == 0
来源：http://jsk.ybcxt.top

[S07] C：数组遍历求和
来源：http://vot.gzhubu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gvh.sufxvd.cn

[S08] C：动态内存分配与释放
来源：http://svt.yfazqb.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ftk.sjlbkw.cn

[S09] C：结构体定义与初始化
来源：http://mfy.shanyushiyangkeji.top


<!-- 参考信息 -->