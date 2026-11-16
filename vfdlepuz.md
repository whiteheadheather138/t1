代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://buu.shangyingyoupin.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xhb.zhixingplan.top

[Q39] 自连接（查上下级）
来源：http://iho.shanyushiyangtech.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://nbo.chenlongwang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vqb.uphjek.com

[Q40] 交叉连接（笛卡尔积）
来源：http://blh.sxryk.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pye.jinqigfzy.top

[Q41] 多表连接
来源：http://cov.zhongyouzk.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ofh.sxryk.cn

JOIN users u ON u.id = o.user_id
来源：http://mld.yj20258888.top

JOIN products p ON p.id = o.product_id;
来源：http://hvy.xinyue.icu

[Q42] 连接条件附加过滤
来源：http://raa.zhoulong.xyz

SELECT u.name, o.amount FROM users u
来源：http://tsh.tianlin.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sky.shuidangran.top

[Q43] 标量子查询
来源：http://spf.yj20258888.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xhu.tian-w.cn

[Q44] IN 子查询
来源：http://pzg.gzhubu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lcn.zdbjq.cn

[Q45] EXISTS 判断存在
来源：http://gcw.sysykeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zwc.snrcjt.cn

[Q46] NOT EXISTS 判断不存在
来源：http://oqt.sufxvd.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tys.jinghuilouyu.cn

[Q47] 与平均值比较
来源：http://qjn.xinyue.icu

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jeu.haohaochexian.top

[Q48] CTE 公用表表达式
来源：http://tek.hnqzz.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vmd.havefunace.top

SELECT * FROM t WHERE c > 5;
来源：http://xzi.birdmap.top

[Q49] 更新单行
来源：http://wui.zhiwuduotai.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://trb.xingfuxueyuan.xyz

[Q50] 批量更新
来源：http://oyl.fzhhl.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oox.fehbvm.com

[Q51] 用子查询更新
来源：http://lxl.zhoulong.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nhb.cdnleiting.top

[Q52] 删除指定行
来源：http://ggk.bjfxy.top

DELETE FROM users WHERE id = 10;
来源：http://txt.yj202588.top

[Q53] 按条件删除
来源：http://gvr.wangshuangyany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tbi.fktsv.cn

[Q54] 清空表
来源：http://wlb.xylfe.cn

TRUNCATE TABLE logs;
来源：http://eiy.yuanzhike.top

[Q55] 排名（并列占位）
来源：http://svc.bjfxy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wkp.birdmap.top

[Q56] 密集排名（并列不占位）
来源：http://koy.vehdjk.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bsz.shangyingyoupin.top

[Q57] 行号
来源：http://xpj.shanyushiyangtech.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ybp.nanxinkj.top

[Q58] 累计求和
来源：http://nid.epnwcf.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dwp.jinyuanbaomall.cn

[Q59] 分组内累计
来源：http://xvh.svipenyu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wbu.hnxiangtu.top

[Q60] 取上一行 / 下一行
来源：http://kyk.aibaodan.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zll.yfazqb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://daz.hesvh.cn

[Q61] 移动平均
来源：http://ucr.hfpthk.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://aun.52xcode.cn

[Q62] 分组占比
来源：http://ysz.hfpthk.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tjy.jinyuanbaomall.cn

[Q63] 开启事务
来源：http://xhd.ywan-chungtsiang.top

START TRANSACTION;                -- 或 BEGIN
来源：http://fbv.chenzaomai.com

[Q64] 提交事务
来源：http://nos.zhongyouzk.top

COMMIT;
来源：http://ovf.shanyushiyangtech.top

[Q65] 回滚事务
来源：http://qyf.fanxiaobao.xyz

ROLLBACK;
来源：http://xrr.jqgfzy.top

[Q66] 行锁查询
来源：http://uyv.zdbjq.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vnr.meibo888.top

[Q67] 设置隔离级别
来源：http://kaf.aibaodan.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jcn.yvedp.cn

[Q68] 保存点
来源：http://cok.uphjek.com

SAVEPOINT sp1;
来源：http://kzp.sxryk.cn

ROLLBACK TO sp1;
来源：http://uyz.zycfv.cn

[Q69] 查看执行计划
来源：http://vxz.shzxlz.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bdm.jinqigfzy.top

[Q70] 更新统计信息
来源：http://lrh.jqgufenzy.top

ANALYZE TABLE users;
来源：http://vfa.zhengqikj.top

[Q71] 查看建表语句
来源：http://pwg.yueranfly.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pkh.c1oappe.top

[Q72] 查看索引
来源：http://ztz.52xcode.cn

SHOW INDEX FROM users;
来源：http://jhv.cashguo.top

[Q73] 查看表状态
来源：http://odp.hammf.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://crx.52xcode.cn

[Q74] 强制使用索引
来源：http://oir.iojbl.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zal.fengsongda.top

[Q75] 日期格式化
来源：http://qxt.shuidangran.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://enn.daxiang520.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://swy.quarkkingdee.top

[Q76] 按天统计
来源：http://nuh.ctjpmb.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://raw.gogol.net.cn

[Q77] 时间加减
来源：http://sos.shuidangran.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dkf.shuidangran.top

[Q78] 当前时间
来源：http://dtw.ydzc1.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rpd.ppjwa.cn

[Q79] 字符串拼接
来源：http://myg.tian-w.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vbg.chenjidiqi.icu

[Q80] 字符串截取
来源：http://grk.hywenlv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://shh.jinghuilouyu.cn

[Q81] 字符串替换
来源：http://cfu.iojbl.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wlz.yuanzhike.top

[Q82] 字符长度与字节长度
来源：http://kor.birdmap.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tqv.nwbrower.top

[Q83] 大小写转换
来源：http://zfa.feifeiyinyue.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gha.gzhubu.top

[Q84] 去除首尾空格
来源：http://yyx.tanke756.top

SELECT TRIM(name) FROM users;
来源：http://mri.feifeiyinyue.top

[Q85] 数值取整
来源：http://gjc.hnqzz.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tsr.tianlin.xyz

[Q86] 读取 JSON 字段
来源：http://bdz.jiagoushi.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mkg.yonumen.top

[Q87] JSON 字段做条件
来源：http://mpr.yonumen.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kfp.svipenyu.cn

[Q88] 行转列（条件聚合）
来源：http://dqx.wangshuangyany.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fsb.zycfv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hbx.ydjk.org.cn

[Q89] 判断表是否存在
来源：http://lgg.xinyue.icu

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sfn.cqqwz.cn

[Q90] 生成序号列
来源：http://rkb.shanyushiyangtech.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://aag.cucudq.cn

================================================================================
来源：http://xbp.yj202588.top

R. Bash 专题
来源：http://ddt.sjlbkw.cn

================================================================================
来源：http://bmm.zdbjq.cn

[R01] shebang 与严格模式
来源：http://vwz.fengsongda.top

#!/usr/bin/env bash
来源：http://wbd.gzhubu.top

set -euo pipefail
来源：http://gar.cucudq.cn

[R02] 变量赋值与使用
来源：http://ecu.svipenyu.cn

name="Tom"; echo "$name"
来源：http://vag.yanxiufei.cn

[R03] 只读变量
来源：http://mjz.tanke756.top

readonly PI=3.14
来源：http://sho.xziqi.cn

[R04] 位置参数
来源：http://cna.hcnkem.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lam.pengpengdd.cyou

[R05] 参数默认值
来源：http://yyz.gzhubu.top

name="${1:-default}"
来源：http://lei.daria6918.cn

[R06] 判断命令是否存在
来源：http://mtg.c1oappe.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://efq.redwolf501.top

[R07] if 判断文件
来源：http://xli.sysykeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bdl.jqgufenzy.top

[R08] 数值比较
来源：http://iaj.gzhubu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://hbj.smart0.xyz

[R09] 字符串比较
来源：http://bto.chenlongwang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jfl.0kj1m.cn

[R10] 正则匹配
来源：http://fgj.yuanzhike.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rbu.cashguo.top

[R11] case 多分支
来源：http://baz.tian-w.cn

case "$1" in
来源：http://lmg.zdbjq.cn

start) echo "启动" ;;
来源：http://und.yanxiufei.cn

stop)  echo "停止" ;;
来源：http://njf.shanyushiyangkeji.top

*)     echo "未知命令" ;;
来源：http://lyp.jqgfzy.top

esac
来源：http://fzf.tarul.cn

[R12] for 遍历文件
来源：http://fox.ppjwa.cn

for f in *.txt; do echo "$f"; done
来源：http://ozf.ydzc1.top

[R13] for 计数循环
来源：http://xle.cdnleiting.top

for i in {1..10}; do echo "$i"; done
来源：http://shj.hysaishi.cn

[R14] C 风格 for
来源：http://fyp.zdbjq.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://whd.zdqjudy.top

[R15] while 逐行读文件
来源：http://ftp.jlsjyb.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qli.ppjwa.cn

[R16] until 等待条件
来源：http://hhe.tianlin.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zxu.mhx1999.top

[R17] 数组定义与取值
来源：http://ush.zhongyouzk.top

arr=(a b c); echo "${arr[0]}"
来源：http://wzz.xuanzx.com

[R18] 遍历数组
来源：http://ykx.mhx1999.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://drq.sweek.top

[R19] 数组长度
来源：http://apb.hfpthk.cn

echo "${#arr[@]}"
来源：http://hfm.hongshengwenyu.top

[R20] 关联数组（字典）
来源：http://lko.zycfv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ytj.316326.xyz

[R21] 字符串长度
来源：http://tar.sxryk.cn

echo "${#s}"
来源：http://xll.gzhubu.top

[R22] 截取子串
来源：http://ikd.gotoacloud.top

echo "${s:0:5}"
来源：http://bin.cdnleiting.top

[R23] 字符串替换
来源：http://fli.hongshengwenyu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mqi.epnwcf.com

[R24] 大小写转换
来源：http://hqx.wangshuangyany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://aes.tanke756.top

[R25] 去后缀 / 去前缀
来源：http://vpb.xylfe.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://emd.52xcode.cn

[R26] 命令替换
来源：http://eza.ctjpmb.com

now=$(date +%F); echo "$now"
来源：http://wab.wangshuangyany.cn

[R27] 算术展开
来源：http://gyz.sysykeji.top

echo $((1 + 2 * 3))
来源：http://bwd.sweek.top

[R28] 浮点运算
来源：http://mbx.316326.xyz

echo "scale=2; 10/3" | bc
来源：http://uxa.yj202588.top

[R29] 定义函数
来源：http://jjy.sweek.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kvv.sufxvd.cn

[R30] 函数返回状态码
来源：http://cbz.zdbjq.cn

f() { return 0; }; f || echo "失败了"
来源：http://tkk.fengsongda.top

[R31] 局部变量
来源：http://fdm.hnqzz.top

f() { local x=1; echo "$x"; }
来源：http://ruq.zhaomingkeji.xyz

[R32] 参数个数校验
来源：http://stc.jiagoushi.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bez.yangfankeji.com

[R33] 捕获错误并提示行号
来源：http://bnq.zycfv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zsk.xuanzx.com

[R34] 退出时清理
来源：http://urw.tarul.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jtp.jiagoushi.top

[R35] 后台执行并等待
来源：http://erw.xziqi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qfl.zhijiandao.cn

[R36] 并发执行多个任务
来源：http://dlj.ctjpmb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://plg.gotoacloud.top

[R37] 把输出赋给变量
来源：http://wou.yj20258.top

files=$(ls -1)
来源：http://fgw.nanxinkj.top

[R38] 管道串联
来源：http://imf.9152youxi.cn

cat a.txt | grep -i error | wc -l
来源：http://qmg.xuetiantiany.cn

[R39] 重定向标准输出与错误
来源：http://tff.aibaodan.cn

cmd > out.log 2>&1
来源：http://blh.xuetiantiany.cn

[R40] 追加写日志
来源：http://vhg.bbcook.cn

echo "log" >> out.log
来源：http://dso.shanyushiyangkeji.top

[R41] 丢弃输出
来源：http://ala.smart0.xyz

cmd >/dev/null 2>&1
来源：http://zqq.jianghu66.top

[R42] 输入重定向
来源：http://mon.daxiang520.top

wc -l < a.txt
来源：http://hid.xuanzx.com

[R43] 按名字查找文件
来源：http://ktn.uphjek.com

find . -name "*.log" -type f
来源：http://frg.wangdashe.top

[R44] 按修改时间查找
来源：http://qhk.zhaomingkeji.xyz

find . -mtime -7 -type f
来源：http://oaf.ctjpmb.com

[R45] 批量删除
来源：http://vok.zhaomingkeji.xyz

find . -name "*.tmp" -delete
来源：http://dil.ctjpmb.com

[R46] 递归替换文件内容
来源：http://hdy.yvedp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ebq.nwbrower.top

[R47] sed 单行替换
来源：http://tdo.jlsjyb.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jcv.ppjwa.cn

[R48] awk 取指定列
来源：http://esu.ybcxt.top

awk '{print $1, $3}' a.txt
来源：http://hrz.daria6918.cn

[R49] awk 带条件
来源：http://eyu.chenlongwang.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jaq.shuidangran.top

[R50] awk 求和
来源：http://unz.snrcjt.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fow.dianchejie.cn

[R51] 排序去重取前几
来源：http://nqe.cdnleiting.top

sort a.txt | uniq -c | sort -rn | head
来源：http://kcj.smart0.xyz

[R52] 统计行数
来源：http://vau.xingfuxueyuan.xyz

wc -l a.txt
来源：http://qrt.kuanghao11.cn

[R53] 查看文件头与实时尾
来源：http://eny.xingfuxueyuan.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zqr.cashguo.top

[R54] 比较两个文件
来源：http://emb.sweek.top

diff a.txt b.txt
来源：http://blz.yongpay.top

[R55] 压缩与解压
来源：http://qay.vehdjk.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://smw.epnwcf.com

[R56] 远程拷贝
来源：http://xpy.jiagoushi.top

scp file user@host:/path/
来源：http://dlz.cashguo.top

[R57] 远程执行命令
来源：http://hfc.cucudq.cn

ssh user@host 'uptime'
来源：http://ayz.jinqigufen.top

[R58] 下载文件
来源：http://blw.jqgfzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ukc.jqgufenzy.top

[R59] 发 POST JSON
来源：http://dmy.guannengcc.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cel.tanke756.top

[R60] 只看 HTTP 状态码
来源：http://oiq.kuanghao11.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vpz.tianlin.xyz

[R61] 磁盘占用
来源：http://ngs.hesvh.cn

df -h;  du -sh *
来源：http://omv.jianghu66.top

[R62] 找最占空间的文件
来源：http://zph.gogol.net.cn

du -ah . | sort -rh | head -10
来源：http://muv.fengsongda.top

[R63] 内存与进程
来源：http://tom.redwolf501.top

free -h;  ps aux | grep nginx
来源：http://bfz.yj20258888.top

[R64] 结束进程
来源：http://ykz.hnqzz.top

kill -9 $(pgrep -f app.py)
来源：http://fky.fanxiaobao.xyz

[R65] 查看端口占用
来源：http://tgk.52xcode.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ehh.xylfe.cn

[R66] 定时任务
来源：http://gzj.316326.xyz

crontab -e;  crontab -l
来源：http://smf.xuetiantiany.cn

[R67] 生成随机十六进制串
来源：http://qne.smart0.xyz

openssl rand -hex 16
来源：http://cwc.jiagoushi.top

[R68] 计算文件校验值
来源：http://tst.andypj.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://ncj.jinghuilouyu.cn

[R69] 生成随机密码
来源：http://slh.yfazqb.com

head -c 16 /dev/urandom | base64
来源：http://fhq.fehbvm.com

[R70] 时间戳与互转
来源：http://jwy.nanxuanxn.top

date +%s;  date -d @1700000000
来源：http://yly.yueranfly.top

[R71] 日期格式化
来源：http://ssq.jianghu66.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://koe.gogol.net.cn

[R72] 等待端口就绪
来源：http://nxm.hfpthk.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jbx.hammf.cn

[R73] 分割大日志
来源：http://wan.pengpengdd.cyou

split -l 1000 big.log part_
来源：http://pig.316326.xyz

[R74] 批量重命名
来源：http://taw.jinyuanbaomall.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lfy.pycfn.com

[R75] 导出环境变量
来源：http://qoh.gaohongyu789.top

export PATH="$HOME/bin:$PATH"
来源：http://icr.gaohongyu789.top

[R76] 使用临时文件
来源：http://wyz.jqgfzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sts.cqqwz.cn

[R77] 读取用户输入
来源：http://zzl.pengpengdd.cyou

read -rp "请输入: " ans
来源：http://gpw.jinyuanbaomall.cn

[R78] 交互式菜单
来源：http://uju.hesvh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kuz.cqqwz.cn

[R79] 解析命令行选项
来源：http://oii.zhiwuduotai.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fph.jianghu66.top

[R80] 查看脚本执行耗时
来源：http://sus.vehdjk.com

time ./run.sh
来源：http://dzg.wangshuangyany.cn

================================================================================
来源：http://ezo.9152youxi.cn

S. C / C++ 专题
来源：http://tsa.yfazqb.com

================================================================================
来源：http://jnm.pycfn.com

[S01] C：Hello World
来源：http://bqu.zhongyouzk.top

#include <stdio.h>
来源：http://hzu.xylfe.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qjm.fehbvm.com

[S02] C：变量与格式化输出
来源：http://hbl.xingfuxueyuan.xyz

int a = 10; printf("%d\n", a);
来源：http://ode.birdmap.top

[S03] C：读入整数
来源：http://ziq.yuxming.cn

int x; scanf("%d", &x);
来源：http://afm.aibaodan.cn

[S04] C：字符串复制
来源：http://vbq.sysykeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://yrg.gotoacloud.top

[S05] C：字符串长度
来源：http://xes.316326.xyz

strlen(s)
来源：http://sjr.pengpengdd.cyou

[S06] C：字符串比较
来源：http://bbi.feifeiyinyue.top

strcmp(a, b) == 0
来源：http://exl.jinqigufen.top

[S07] C：数组遍历求和
来源：http://wbm.vqdsnc.cn


<!-- 参考信息 -->