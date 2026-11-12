代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://efv.quarkkingdee.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kqp.zhoulong.xyz

[Q43] 标量子查询
来源：http://rnn.shuidangran.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vun.hesvh.cn

[Q44] IN 子查询
来源：http://agm.fzhhl.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jry.nwbrower.top

[Q45] EXISTS 判断存在
来源：http://mju.sweek.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xqx.daxiang520.top

[Q46] NOT EXISTS 判断不存在
来源：http://qia.hfpthk.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kwg.cqqwz.cn

[Q47] 与平均值比较
来源：http://bcm.sjlbkw.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ntv.zhengqikj.top

[Q48] CTE 公用表表达式
来源：http://exl.shanyushiyangkeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hqv.zhongyouzk.top

SELECT * FROM t WHERE c > 5;
来源：http://hvk.yj202588.top

[Q49] 更新单行
来源：http://gti.hammf.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://onv.haohaochexian.top

[Q50] 批量更新
来源：http://esv.shuidangran.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zmn.fktsv.cn

[Q51] 用子查询更新
来源：http://qio.daria6918.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://beb.zdqjudy.top

[Q52] 删除指定行
来源：http://yki.gzhubu.top

DELETE FROM users WHERE id = 10;
来源：http://mfa.hesvh.cn

[Q53] 按条件删除
来源：http://wxy.iojbl.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oiq.yanxiufei.cn

[Q54] 清空表
来源：http://rid.xylfe.cn

TRUNCATE TABLE logs;
来源：http://spq.hnqzz.top

[Q55] 排名（并列占位）
来源：http://frs.yangfankeji.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gtc.fengsongda.top

[Q56] 密集排名（并列不占位）
来源：http://bex.chenjidiqi.icu

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://iqa.jqgufenzy.top

[Q57] 行号
来源：http://vvo.hammf.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jbj.cqqwz.cn

[Q58] 累计求和
来源：http://hvx.daria6918.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hux.yueranfly.top

[Q59] 分组内累计
来源：http://dzg.yanxiufei.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yuj.0kj1m.cn

[Q60] 取上一行 / 下一行
来源：http://vhy.jinqigfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hlx.shzxlz.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://eqb.sysykeji.top

[Q61] 移动平均
来源：http://kze.fzhhl.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dts.aibaodan.cn

[Q62] 分组占比
来源：http://yph.jinqigufen.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://erb.yj20258888.top

[Q63] 开启事务
来源：http://kxe.nwbrower.top

START TRANSACTION;                -- 或 BEGIN
来源：http://uec.hnxiangtu.top

[Q64] 提交事务
来源：http://tlt.cheryme.top

COMMIT;
来源：http://gbn.fengsongda.top

[Q65] 回滚事务
来源：http://fnw.ywan-chungtsiang.top

ROLLBACK;
来源：http://ylo.jinqigufen.top

[Q66] 行锁查询
来源：http://uma.smart0.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ivr.ywan-chungtsiang.top

[Q67] 设置隔离级别
来源：http://xdf.sysykeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://klk.dianchejie.cn

[Q68] 保存点
来源：http://txh.uphjek.com

SAVEPOINT sp1;
来源：http://esg.zdbjq.cn

ROLLBACK TO sp1;
来源：http://rgg.shangyingyoupin.top

[Q69] 查看执行计划
来源：http://pca.shanyushiyangtech.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wde.tian-w.cn

[Q70] 更新统计信息
来源：http://pgr.zhoulong.xyz

ANALYZE TABLE users;
来源：http://lcd.ivvv.top

[Q71] 查看建表语句
来源：http://asw.shzxlz.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://efd.zhengqikj.top

[Q72] 查看索引
来源：http://bvy.aizwys.cn

SHOW INDEX FROM users;
来源：http://krd.hfpthk.cn

[Q73] 查看表状态
来源：http://woz.yanxiufei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rzh.chenjidiqi.icu

[Q74] 强制使用索引
来源：http://ujs.hnqzz.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xmf.guowangkeji.top

[Q75] 日期格式化
来源：http://wlx.aibaodan.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fkh.zhoulong.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sni.redwolf501.top

[Q76] 按天统计
来源：http://zby.bjfxy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rdu.nanxinkj.top

[Q77] 时间加减
来源：http://olg.hesvh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gkj.haohaochexian.top

[Q78] 当前时间
来源：http://ani.ppjwa.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bmf.hesvh.cn

[Q79] 字符串拼接
来源：http://bzh.fzhhl.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://chg.pengpengdd.cyou

[Q80] 字符串截取
来源：http://xbg.shanyushiyangkeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://myi.chenlongwang.top

[Q81] 字符串替换
来源：http://vzl.hywenlv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rsh.shanyushiyangkeji.top

[Q82] 字符长度与字节长度
来源：http://abq.hnqzz.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://how.guannengcc.top

[Q83] 大小写转换
来源：http://zni.yj20258888.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hvg.jyoumei.cn

[Q84] 去除首尾空格
来源：http://rva.hywenlv.cn

SELECT TRIM(name) FROM users;
来源：http://vvt.daxiang520.top

[Q85] 数值取整
来源：http://huv.andypj.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://taf.daria6918.cn

[Q86] 读取 JSON 字段
来源：http://qny.yuxming.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ywb.ybcxt.top

[Q87] JSON 字段做条件
来源：http://aje.gaohongyu789.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lam.ybcxt.top

[Q88] 行转列（条件聚合）
来源：http://ymf.jqgfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sdf.yanxiufei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gve.jyoumei.cn

[Q89] 判断表是否存在
来源：http://wzn.zhongyouzk.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kzh.yuanzhike.top

[Q90] 生成序号列
来源：http://kog.316326.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vji.yj20258.top

================================================================================
来源：http://jmm.daxiang520.top

R. Bash 专题
来源：http://lnl.yongpay.top

================================================================================
来源：http://efs.9152youxi.cn

[R01] shebang 与严格模式
来源：http://lqk.shangyingyoupin.top

#!/usr/bin/env bash
来源：http://axm.cucudq.cn

set -euo pipefail
来源：http://sum.nwbrower.top

[R02] 变量赋值与使用
来源：http://yte.fanxiaobao.xyz

name="Tom"; echo "$name"
来源：http://kuc.tianlin.xyz

[R03] 只读变量
来源：http://xgg.vqdsnc.cn

readonly PI=3.14
来源：http://wxl.xziqi.cn

[R04] 位置参数
来源：http://awm.zhiwuduotai.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nay.fzhhl.top

[R05] 参数默认值
来源：http://lja.hnqzz.top

name="${1:-default}"
来源：http://dqk.xuanzx.com

[R06] 判断命令是否存在
来源：http://mjd.zhixingplan.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://chz.guowangkeji.top

[R07] if 判断文件
来源：http://wob.ivvv.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://msr.bjfxy.top

[R08] 数值比较
来源：http://yup.cheryme.top

if (( a > b )); then echo "a 更大"; fi
来源：http://usj.tanke756.top

[R09] 字符串比较
来源：http://kjy.xinyue.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://soh.jiagoushi.top

[R10] 正则匹配
来源：http://krr.xingfuxueyuan.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tuw.jiagoushi.top

[R11] case 多分支
来源：http://cbs.sufxvd.cn

case "$1" in
来源：http://wrl.yj20258.top

start) echo "启动" ;;
来源：http://dds.zhixingplan.top

stop)  echo "停止" ;;
来源：http://axk.nanxuanxn.top

*)     echo "未知命令" ;;
来源：http://ewt.wangdashe.top

esac
来源：http://wqw.hcnkem.com

[R12] for 遍历文件
来源：http://aje.tianlin.xyz

for f in *.txt; do echo "$f"; done
来源：http://dtz.ehwqpu.com

[R13] for 计数循环
来源：http://svg.guannengcc.top

for i in {1..10}; do echo "$i"; done
来源：http://wlc.yj20258888.top

[R14] C 风格 for
来源：http://qbk.jinghuilouyu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yyl.daria6918.cn

[R15] while 逐行读文件
来源：http://gnt.sjlbkw.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://eia.yj20258888.top

[R16] until 等待条件
来源：http://zlz.yj202588.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ssi.jinqigufen.top

[R17] 数组定义与取值
来源：http://uiz.zhixingplan.top

arr=(a b c); echo "${arr[0]}"
来源：http://mjv.jinqigfzy.top

[R18] 遍历数组
来源：http://ddp.xingfuxueyuan.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ywi.52xcode.cn

[R19] 数组长度
来源：http://fog.hongshengwenyu.top

echo "${#arr[@]}"
来源：http://vbd.yangfankeji.com

[R20] 关联数组（字典）
来源：http://xle.sxryk.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rgq.havefunace.top

[R21] 字符串长度
来源：http://xjn.vehdjk.com

echo "${#s}"
来源：http://zag.pycfn.com

[R22] 截取子串
来源：http://dhm.gzhubu.top

echo "${s:0:5}"
来源：http://nfq.vqdsnc.cn

[R23] 字符串替换
来源：http://zqi.snrcjt.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vmk.chenjidiqi.icu

[R24] 大小写转换
来源：http://tie.jinghuilouyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yqr.yuxming.cn

[R25] 去后缀 / 去前缀
来源：http://ykv.feifeiyinyue.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://pmy.jqgufenzy.top

[R26] 命令替换
来源：http://jqd.jinyuanbaomall.cn

now=$(date +%F); echo "$now"
来源：http://pdp.tanke756.top

[R27] 算术展开
来源：http://kam.xingfuxueyuan.xyz

echo $((1 + 2 * 3))
来源：http://mro.yfazqb.com

[R28] 浮点运算
来源：http://iei.yuanzhike.top

echo "scale=2; 10/3" | bc
来源：http://kfh.sysykeji.top

[R29] 定义函数
来源：http://mef.hammf.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gxi.jqgfzy.top

[R30] 函数返回状态码
来源：http://djg.jiagoushi.top

f() { return 0; }; f || echo "失败了"
来源：http://okd.hysaishi.cn

[R31] 局部变量
来源：http://suy.yangfankeji.com

f() { local x=1; echo "$x"; }
来源：http://ldc.0kj1m.cn

[R32] 参数个数校验
来源：http://wcv.sweek.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wiv.redwolf501.top

[R33] 捕获错误并提示行号
来源：http://sbi.xuetiantiany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eef.smart0.xyz

[R34] 退出时清理
来源：http://tdc.hywenlv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fcy.gogol.net.cn

[R35] 后台执行并等待
来源：http://rvi.0kj1m.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://urm.iojbl.cn

[R36] 并发执行多个任务
来源：http://dxl.zycfv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bsy.zhixingplan.top

[R37] 把输出赋给变量
来源：http://zao.sweek.top

files=$(ls -1)
来源：http://rku.uphjek.com

[R38] 管道串联
来源：http://plo.fehbvm.com

cat a.txt | grep -i error | wc -l
来源：http://npx.shzxlz.cn

[R39] 重定向标准输出与错误
来源：http://xhj.zdqjudy.top

cmd > out.log 2>&1
来源：http://awv.ehwqpu.com

[R40] 追加写日志
来源：http://gqv.zdqjudy.top

echo "log" >> out.log
来源：http://ohc.wangshuangyany.cn

[R41] 丢弃输出
来源：http://yib.pycfn.com

cmd >/dev/null 2>&1
来源：http://crb.yuanzhike.top

[R42] 输入重定向
来源：http://mqg.sweek.top

wc -l < a.txt
来源：http://yil.birdmap.top

[R43] 按名字查找文件
来源：http://ukl.aibaodan.cn

find . -name "*.log" -type f
来源：http://bww.zhengqikj.top

[R44] 按修改时间查找
来源：http://pjc.chenjidiqi.icu

find . -mtime -7 -type f
来源：http://dwl.xuetiantiany.cn

[R45] 批量删除
来源：http://ysj.daria6918.cn

find . -name "*.tmp" -delete
来源：http://dlm.feifeiyinyue.top

[R46] 递归替换文件内容
来源：http://idi.xylfe.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ltv.yj20258.top

[R47] sed 单行替换
来源：http://rai.daxiang520.top

sed -i 's/foo/bar/g' a.txt
来源：http://odu.xziqi.cn

[R48] awk 取指定列
来源：http://rod.cucudq.cn

awk '{print $1, $3}' a.txt
来源：http://fld.cheryme.top

[R49] awk 带条件
来源：http://avc.zhaomingkeji.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fav.jinghuilouyu.cn

[R50] awk 求和
来源：http://piu.cheryme.top

awk '{s += $2} END {print s}' a.txt
来源：http://nvr.zhijiandao.cn

[R51] 排序去重取前几
来源：http://bex.zhengqikj.top

sort a.txt | uniq -c | sort -rn | head
来源：http://sow.ehwqpu.com

[R52] 统计行数
来源：http://rgu.feifeiyinyue.top

wc -l a.txt
来源：http://cim.xziqi.cn

[R53] 查看文件头与实时尾
来源：http://nuw.jinqigfzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://klb.hysaishi.cn

[R54] 比较两个文件
来源：http://xfc.yanxiufei.cn

diff a.txt b.txt
来源：http://rhv.yvedp.cn

[R55] 压缩与解压
来源：http://hko.9152youxi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://djb.yangfankeji.com

[R56] 远程拷贝
来源：http://fir.wangdashe.top

scp file user@host:/path/
来源：http://cha.dashuyun.cn

[R57] 远程执行命令
来源：http://rqw.haohaochexian.top

ssh user@host 'uptime'
来源：http://bqo.xuetiantiany.cn

[R58] 下载文件
来源：http://rai.yueranfly.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bzq.jinqigfzy.top

[R59] 发 POST JSON
来源：http://yml.vqdsnc.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ppk.shuidangran.top

[R60] 只看 HTTP 状态码
来源：http://vpl.cashguo.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fzh.epnwcf.com

[R61] 磁盘占用
来源：http://tdx.feifeiyinyue.top

df -h;  du -sh *
来源：http://rhd.yfazqb.com

[R62] 找最占空间的文件
来源：http://reo.shanyushiyangkeji.top

du -ah . | sort -rh | head -10
来源：http://iln.vehdjk.com

[R63] 内存与进程
来源：http://ktl.ppjwa.cn

free -h;  ps aux | grep nginx
来源：http://see.zhaomingkeji.xyz

[R64] 结束进程
来源：http://bha.vqdsnc.cn

kill -9 $(pgrep -f app.py)
来源：http://yuy.nanxuanxn.top

[R65] 查看端口占用
来源：http://rtz.bbcook.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dmi.sweek.top

[R66] 定时任务
来源：http://tmx.c1oappe.top

crontab -e;  crontab -l
来源：http://yzj.tianlin.xyz

[R67] 生成随机十六进制串
来源：http://bsg.quarkkingdee.top

openssl rand -hex 16
来源：http://vip.cashguo.top

[R68] 计算文件校验值
来源：http://tnm.iojbl.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ret.shuidangran.top

[R69] 生成随机密码
来源：http://xdn.yangfankeji.com

head -c 16 /dev/urandom | base64
来源：http://lbw.wangdashe.top

[R70] 时间戳与互转
来源：http://occ.zhoulong.xyz

date +%s;  date -d @1700000000
来源：http://uau.cashguo.top

[R71] 日期格式化
来源：http://bnt.xylfe.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lkc.52xcode.cn

[R72] 等待端口就绪
来源：http://vcl.jianghu66.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fgd.tarul.cn

[R73] 分割大日志
来源：http://hte.9152youxi.cn

split -l 1000 big.log part_
来源：http://ccr.birdmap.top

[R74] 批量重命名
来源：http://bsv.tian-w.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zoa.daria6918.cn

[R75] 导出环境变量
来源：http://aoo.tian-w.cn

export PATH="$HOME/bin:$PATH"
来源：http://ynk.yueranfly.top

[R76] 使用临时文件
来源：http://ats.tianlin.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://iuh.feifeiyinyue.top

[R77] 读取用户输入
来源：http://htg.fengsongda.top

read -rp "请输入: " ans
来源：http://ftb.xuanzx.com

[R78] 交互式菜单
来源：http://lwe.daxiang520.top

select opt in a b c; do echo "$opt"; break; done
来源：http://cdy.zdbjq.cn

[R79] 解析命令行选项
来源：http://gzt.316326.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rsr.quarkkingdee.top

[R80] 查看脚本执行耗时
来源：http://yzw.yanxiufei.cn

time ./run.sh
来源：http://dxa.daria6918.cn

================================================================================
来源：http://dyp.hammf.cn

S. C / C++ 专题
来源：http://ogq.vehdjk.com

================================================================================
来源：http://vho.ywan-chungtsiang.top

[S01] C：Hello World
来源：http://jso.xuanzx.com

#include <stdio.h>
来源：http://lwz.chenjidiqi.icu

int main(void) { printf("Hello\n"); return 0; }
来源：http://dhc.yfazqb.com

[S02] C：变量与格式化输出
来源：http://lzj.dianchejie.cn

int a = 10; printf("%d\n", a);
来源：http://eej.fehbvm.com

[S03] C：读入整数
来源：http://icb.gogol.net.cn

int x; scanf("%d", &x);
来源：http://ybb.smart0.xyz

[S04] C：字符串复制
来源：http://kbw.bbcook.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tsm.xingfuxueyuan.xyz

[S05] C：字符串长度
来源：http://dta.yueranfly.top

strlen(s)
来源：http://qlb.chenjidiqi.icu

[S06] C：字符串比较
来源：http://nhf.zhiwuduotai.top

strcmp(a, b) == 0
来源：http://dmy.yj20258.top

[S07] C：数组遍历求和
来源：http://cdg.yvedp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xgg.yfazqb.com

[S08] C：动态内存分配与释放
来源：http://rfk.cucudq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://abe.cashguo.top

[S09] C：结构体定义与初始化
来源：http://pyj.jinghuilouyu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kpl.hcnkem.com

[S10] C：指针与解引用
来源：http://pox.cucudq.cn

int *p = &a;  *p = 5;
来源：http://aar.jinqigufen.top

[S11] C：逐行读文件
来源：http://xla.wangshuangyany.cn

FILE *f = fopen("a.txt", "r");
来源：http://ezg.yvedp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tyb.epnwcf.com

fclose(f);
来源：http://ugy.zhoulong.xyz

[S12] C：写文件
来源：http://tyj.yj20258888.top


<!-- 参考信息 -->