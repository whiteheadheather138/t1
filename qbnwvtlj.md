代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kli.sxryk.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dwo.ybcxt.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yqy.cheryme.top

[Q41] 多表连接
来源：http://aaj.zhongyouzk.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://qmt.xuetiantiany.cn

JOIN users u ON u.id = o.user_id
来源：http://ybu.fehbvm.com

JOIN products p ON p.id = o.product_id;
来源：http://fat.fzhhl.top

[Q42] 连接条件附加过滤
来源：http://bcj.jinqigufen.top

SELECT u.name, o.amount FROM users u
来源：http://lhw.ydjk.org.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vxy.jinyuanbaomall.cn

[Q43] 标量子查询
来源：http://mla.ppjwa.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lem.fktsv.cn

[Q44] IN 子查询
来源：http://zfv.jinqigfzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xpw.jinghuilouyu.cn

[Q45] EXISTS 判断存在
来源：http://qnl.sxryk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fhr.sjlbkw.cn

[Q46] NOT EXISTS 判断不存在
来源：http://eox.svipenyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cwv.ybcxt.top

[Q47] 与平均值比较
来源：http://lrz.shanyushiyangkeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uxv.zhiwuduotai.top

[Q48] CTE 公用表表达式
来源：http://wjn.fengsongda.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qwh.yueranfly.top

SELECT * FROM t WHERE c > 5;
来源：http://lkm.hammf.cn

[Q49] 更新单行
来源：http://egd.wangdashe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://aje.aibaodan.cn

[Q50] 批量更新
来源：http://gsr.yongpay.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yee.havefunace.top

[Q51] 用子查询更新
来源：http://ksz.chenzaomai.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://aiy.yonumen.top

[Q52] 删除指定行
来源：http://wrm.fzhhl.top

DELETE FROM users WHERE id = 10;
来源：http://esn.tarul.cn

[Q53] 按条件删除
来源：http://kbx.ybcxt.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oew.birdmap.top

[Q54] 清空表
来源：http://wqi.daxiang520.top

TRUNCATE TABLE logs;
来源：http://urm.yuanzhike.top

[Q55] 排名（并列占位）
来源：http://cnq.sweek.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uxx.hysaishi.cn

[Q56] 密集排名（并列不占位）
来源：http://xnb.jianghu66.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gqh.mhx1999.top

[Q57] 行号
来源：http://ycd.zhiwuduotai.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://udj.gotoacloud.top

[Q58] 累计求和
来源：http://llt.ydjk.org.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tul.jlsjyb.cn

[Q59] 分组内累计
来源：http://fdd.jianghu66.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sag.yueranfly.top

[Q60] 取上一行 / 下一行
来源：http://ixp.zhiwuduotai.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://unk.shuidangran.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://huw.hfpthk.cn

[Q61] 移动平均
来源：http://rkj.vqdsnc.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bzm.kuanghao11.cn

[Q62] 分组占比
来源：http://rax.jlsjyb.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fbd.jqgfzy.top

[Q63] 开启事务
来源：http://xyv.kuanghao11.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://org.shuidangran.top

[Q64] 提交事务
来源：http://pem.zhoulong.xyz

COMMIT;
来源：http://oic.haohaochexian.top

[Q65] 回滚事务
来源：http://kmu.gogol.net.cn

ROLLBACK;
来源：http://wuk.nwbrower.top

[Q66] 行锁查询
来源：http://sse.fanxiaobao.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gta.shzxlz.cn

[Q67] 设置隔离级别
来源：http://opu.gaohongyu789.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://txm.feifeiyinyue.top

[Q68] 保存点
来源：http://ysb.wangdashe.top

SAVEPOINT sp1;
来源：http://jzc.gaohongyu789.top

ROLLBACK TO sp1;
来源：http://wdo.tian-w.cn

[Q69] 查看执行计划
来源：http://jtj.hesvh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xgw.yangfankeji.com

[Q70] 更新统计信息
来源：http://vgw.redwolf501.top

ANALYZE TABLE users;
来源：http://bzd.316326.xyz

[Q71] 查看建表语句
来源：http://uvp.zdbjq.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ppq.mhx1999.top

[Q72] 查看索引
来源：http://lfd.52xcode.cn

SHOW INDEX FROM users;
来源：http://pew.zycfv.cn

[Q73] 查看表状态
来源：http://wde.yueranfly.top

SHOW TABLE STATUS LIKE 'users';
来源：http://gmw.ydjk.org.cn

[Q74] 强制使用索引
来源：http://yry.zhongyouzk.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ltn.jqgfzy.top

[Q75] 日期格式化
来源：http://wmp.zhoulong.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hyt.hnxiangtu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mcu.meibo888.top

[Q76] 按天统计
来源：http://byy.shuidangran.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xmt.chenjidiqi.icu

[Q77] 时间加减
来源：http://sdj.aizwys.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://avw.guannengcc.top

[Q78] 当前时间
来源：http://fvl.kuanghao11.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://swi.haohaochexian.top

[Q79] 字符串拼接
来源：http://qli.yuanzhike.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vxm.ywan-chungtsiang.top

[Q80] 字符串截取
来源：http://eeb.hesvh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uns.mhx1999.top

[Q81] 字符串替换
来源：http://tjo.shanyushiyangtech.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kec.fktsv.cn

[Q82] 字符长度与字节长度
来源：http://bgz.yfazqb.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tmz.0kj1m.cn

[Q83] 大小写转换
来源：http://qri.jiagoushi.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qay.pengpengdd.cyou

[Q84] 去除首尾空格
来源：http://gtg.jinghuilouyu.cn

SELECT TRIM(name) FROM users;
来源：http://uak.tian-w.cn

[Q85] 数值取整
来源：http://thm.jiagoushi.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sqx.hfpthk.cn

[Q86] 读取 JSON 字段
来源：http://vlf.daxiang520.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zsh.zhiwuduotai.top

[Q87] JSON 字段做条件
来源：http://saf.sysykeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zxa.tianlin.xyz

[Q88] 行转列（条件聚合）
来源：http://qfi.haohaochexian.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bkc.yangfankeji.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://aza.zdbjq.cn

[Q89] 判断表是否存在
来源：http://een.aizwys.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kqt.zhaomingkeji.xyz

[Q90] 生成序号列
来源：http://yyd.ywan-chungtsiang.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hsg.daxiang520.top

================================================================================
来源：http://bwb.redwolf501.top

R. Bash 专题
来源：http://vpg.0kj1m.cn

================================================================================
来源：http://hsg.yuxming.cn

[R01] shebang 与严格模式
来源：http://qoz.gzhubu.top

#!/usr/bin/env bash
来源：http://hlr.jinqigufen.top

set -euo pipefail
来源：http://fpc.yangfankeji.com

[R02] 变量赋值与使用
来源：http://iob.shanyushiyangtech.top

name="Tom"; echo "$name"
来源：http://cvz.xuanzx.com

[R03] 只读变量
来源：http://vka.sufxvd.cn

readonly PI=3.14
来源：http://hpo.redwolf501.top

[R04] 位置参数
来源：http://has.yueranfly.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bzo.ivvv.top

[R05] 参数默认值
来源：http://jrg.guannengcc.top

name="${1:-default}"
来源：http://jtw.cdnleiting.top

[R06] 判断命令是否存在
来源：http://ebd.yfazqb.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ylg.zhengqikj.top

[R07] if 判断文件
来源：http://hxp.xziqi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vbw.hcnkem.com

[R08] 数值比较
来源：http://rjm.wangshuangyany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fqh.jianghu66.top

[R09] 字符串比较
来源：http://tqd.nanxinkj.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mbv.jinqigufen.top

[R10] 正则匹配
来源：http://dui.mhx1999.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hrn.zhoulong.xyz

[R11] case 多分支
来源：http://tqd.pycfn.com

case "$1" in
来源：http://gnj.yuxming.cn

start) echo "启动" ;;
来源：http://lbm.hfpthk.cn

stop)  echo "停止" ;;
来源：http://hod.shuidangran.top

*)     echo "未知命令" ;;
来源：http://xtk.zycfv.cn

esac
来源：http://mqx.dianchejie.cn

[R12] for 遍历文件
来源：http://epe.quarkkingdee.top

for f in *.txt; do echo "$f"; done
来源：http://eni.aibaodan.cn

[R13] for 计数循环
来源：http://mjs.epnwcf.com

for i in {1..10}; do echo "$i"; done
来源：http://zdz.daria6918.cn

[R14] C 风格 for
来源：http://bbf.jiagoushi.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uzl.shanyushiyangtech.top

[R15] while 逐行读文件
来源：http://zvk.316326.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rzz.jinyuanbaomall.cn

[R16] until 等待条件
来源：http://wtc.wangshuangyany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vbr.ybcxt.top

[R17] 数组定义与取值
来源：http://egz.epnwcf.com

arr=(a b c); echo "${arr[0]}"
来源：http://agi.shanyushiyangkeji.top

[R18] 遍历数组
来源：http://pbv.quarkkingdee.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mun.daria6918.cn

[R19] 数组长度
来源：http://ykq.snrcjt.cn

echo "${#arr[@]}"
来源：http://vwd.cashguo.top

[R20] 关联数组（字典）
来源：http://pxu.tanke756.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://iom.tian-w.cn

[R21] 字符串长度
来源：http://ioy.mhx1999.top

echo "${#s}"
来源：http://nlb.cheryme.top

[R22] 截取子串
来源：http://pim.bbcook.cn

echo "${s:0:5}"
来源：http://bgo.tanke756.top

[R23] 字符串替换
来源：http://vfb.redwolf501.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hxp.cucudq.cn

[R24] 大小写转换
来源：http://isi.zdbjq.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ovg.jinghuilouyu.cn

[R25] 去后缀 / 去前缀
来源：http://jtg.zhijiandao.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kba.sweek.top

[R26] 命令替换
来源：http://ezu.aizwys.cn

now=$(date +%F); echo "$now"
来源：http://lbi.epnwcf.com

[R27] 算术展开
来源：http://xbe.chenlongwang.top

echo $((1 + 2 * 3))
来源：http://jpd.jqgfzy.top

[R28] 浮点运算
来源：http://kln.havefunace.top

echo "scale=2; 10/3" | bc
来源：http://rge.yonumen.top

[R29] 定义函数
来源：http://gkp.ydzc1.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nic.yj20258888.top

[R30] 函数返回状态码
来源：http://bao.daria6918.cn

f() { return 0; }; f || echo "失败了"
来源：http://qwk.snrcjt.cn

[R31] 局部变量
来源：http://oav.zhoulong.xyz

f() { local x=1; echo "$x"; }
来源：http://nvx.vqdsnc.cn

[R32] 参数个数校验
来源：http://ykz.kuanghao11.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ell.yangfankeji.com

[R33] 捕获错误并提示行号
来源：http://eak.chenzaomai.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://igy.ybcxt.top

[R34] 退出时清理
来源：http://gcv.sxryk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nsn.hesvh.cn

[R35] 后台执行并等待
来源：http://sso.zhengqikj.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dtj.epnwcf.com

[R36] 并发执行多个任务
来源：http://rgk.jinqigufen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lct.wangshuangyany.cn

[R37] 把输出赋给变量
来源：http://kfm.ivvv.top

files=$(ls -1)
来源：http://qav.xinyue.icu

[R38] 管道串联
来源：http://hlc.jinyuanbaomall.cn

cat a.txt | grep -i error | wc -l
来源：http://rvg.yuanzhike.top

[R39] 重定向标准输出与错误
来源：http://xby.nanxinkj.top

cmd > out.log 2>&1
来源：http://jwh.zhijiandao.cn

[R40] 追加写日志
来源：http://bvn.tarul.cn

echo "log" >> out.log
来源：http://nlv.yonumen.top

[R41] 丢弃输出
来源：http://xje.xuanzx.com

cmd >/dev/null 2>&1
来源：http://ziu.nanxinkj.top

[R42] 输入重定向
来源：http://wxe.hnxiangtu.top

wc -l < a.txt
来源：http://fgq.jinyuanbaomall.cn

[R43] 按名字查找文件
来源：http://gkg.sweek.top

find . -name "*.log" -type f
来源：http://jsx.hammf.cn

[R44] 按修改时间查找
来源：http://crh.chenlongwang.top

find . -mtime -7 -type f
来源：http://vhw.sysykeji.top

[R45] 批量删除
来源：http://hvw.andypj.xyz

find . -name "*.tmp" -delete
来源：http://mxg.ydjk.org.cn

[R46] 递归替换文件内容
来源：http://rdg.yuanzhike.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://boi.ydzc1.top

[R47] sed 单行替换
来源：http://zef.pengpengdd.cyou

sed -i 's/foo/bar/g' a.txt
来源：http://pqi.jyoumei.cn

[R48] awk 取指定列
来源：http://cyd.yuxming.cn

awk '{print $1, $3}' a.txt
来源：http://plz.zhixingplan.top

[R49] awk 带条件
来源：http://ctz.sweek.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gbz.ydzc1.top

[R50] awk 求和
来源：http://ruc.cdnleiting.top

awk '{s += $2} END {print s}' a.txt
来源：http://ysc.mhx1999.top

[R51] 排序去重取前几
来源：http://olj.zdqjudy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://nhh.tianlin.xyz

[R52] 统计行数
来源：http://qis.jyoumei.cn

wc -l a.txt
来源：http://vwa.ywan-chungtsiang.top

[R53] 查看文件头与实时尾
来源：http://mpz.havefunace.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pnv.vehdjk.com

[R54] 比较两个文件
来源：http://zde.gotoacloud.top

diff a.txt b.txt
来源：http://kpa.sjlbkw.cn

[R55] 压缩与解压
来源：http://rbs.zhijiandao.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://all.xylfe.cn

[R56] 远程拷贝
来源：http://jzm.epnwcf.com

scp file user@host:/path/
来源：http://yuh.fengsongda.top

[R57] 远程执行命令
来源：http://kal.dashuyun.cn

ssh user@host 'uptime'
来源：http://nrh.bjfxy.top

[R58] 下载文件
来源：http://gmf.cheryme.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yfe.shanyushiyangkeji.top

[R59] 发 POST JSON
来源：http://wnw.yangfankeji.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nfp.hnqzz.top

[R60] 只看 HTTP 状态码
来源：http://xvd.fehbvm.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wpo.epnwcf.com

[R61] 磁盘占用
来源：http://toc.zhijiandao.cn

df -h;  du -sh *
来源：http://ymi.jiagoushi.top

[R62] 找最占空间的文件
来源：http://kxd.shanyushiyangkeji.top

du -ah . | sort -rh | head -10
来源：http://nqz.yvedp.cn

[R63] 内存与进程
来源：http://obp.tanke756.top

free -h;  ps aux | grep nginx
来源：http://nrs.kuanghao11.cn

[R64] 结束进程
来源：http://byw.mhx1999.top

kill -9 $(pgrep -f app.py)
来源：http://xfj.fehbvm.com

[R65] 查看端口占用
来源：http://lcs.snrcjt.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://crk.hywenlv.cn

[R66] 定时任务
来源：http://kfy.hesvh.cn

crontab -e;  crontab -l
来源：http://pbg.ivvv.top

[R67] 生成随机十六进制串
来源：http://tmk.ehwqpu.com

openssl rand -hex 16
来源：http://cde.52xcode.cn

[R68] 计算文件校验值
来源：http://fpj.vqdsnc.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nhe.zdqjudy.top

[R69] 生成随机密码
来源：http://ymr.hammf.cn

head -c 16 /dev/urandom | base64
来源：http://ots.chenzaomai.com

[R70] 时间戳与互转
来源：http://vew.cheryme.top

date +%s;  date -d @1700000000
来源：http://qky.yfazqb.com

[R71] 日期格式化
来源：http://nus.ctjpmb.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://xch.yuxming.cn

[R72] 等待端口就绪
来源：http://rwv.jinyuanbaomall.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ayy.fzhhl.top

[R73] 分割大日志
来源：http://dog.birdmap.top

split -l 1000 big.log part_
来源：http://oru.yuanzhike.top

[R74] 批量重命名
来源：http://ddm.cucudq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vvv.hfpthk.cn

[R75] 导出环境变量
来源：http://dbm.sufxvd.cn

export PATH="$HOME/bin:$PATH"
来源：http://bub.aibaodan.cn

[R76] 使用临时文件
来源：http://hly.dianchejie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hli.xuanzx.com

[R77] 读取用户输入
来源：http://aqz.dashuyun.cn

read -rp "请输入: " ans
来源：http://zge.mhx1999.top

[R78] 交互式菜单
来源：http://tlt.cucudq.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kse.jianghu66.top

[R79] 解析命令行选项
来源：http://eqa.birdmap.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sxy.vehdjk.com

[R80] 查看脚本执行耗时
来源：http://xzr.zdqjudy.top

time ./run.sh
来源：http://spm.cashguo.top

================================================================================
来源：http://gyu.yuanzhike.top

S. C / C++ 专题
来源：http://etv.zhiwuduotai.top

================================================================================
来源：http://euw.sweek.top

[S01] C：Hello World
来源：http://hrf.hongshengwenyu.top

#include <stdio.h>
来源：http://tdp.kuanghao11.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kfr.wangshuangyany.cn

[S02] C：变量与格式化输出
来源：http://plg.c1oappe.top

int a = 10; printf("%d\n", a);
来源：http://uel.cqqwz.cn

[S03] C：读入整数
来源：http://qhp.tianlin.xyz

int x; scanf("%d", &x);
来源：http://hrv.fzhhl.top

[S04] C：字符串复制
来源：http://wxq.sysykeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://cgf.vehdjk.com

[S05] C：字符串长度
来源：http://iky.gzhubu.top

strlen(s)
来源：http://lam.yonumen.top

[S06] C：字符串比较
来源：http://fcp.c1oappe.top

strcmp(a, b) == 0
来源：http://tsc.tanke756.top

[S07] C：数组遍历求和
来源：http://mfh.ywan-chungtsiang.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bga.fzhhl.top

[S08] C：动态内存分配与释放
来源：http://tdt.ctjpmb.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mhl.jyoumei.cn

[S09] C：结构体定义与初始化
来源：http://gbl.sweek.top


<!-- 参考信息 -->