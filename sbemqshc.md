代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://eje.jinghuilouyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://col.zhoulong.xyz

[Q47] 与平均值比较
来源：http://abl.hesvh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vga.vqdsnc.cn

[Q48] CTE 公用表表达式
来源：http://lne.9152youxi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mhu.ctjpmb.com

SELECT * FROM t WHERE c > 5;
来源：http://njx.jinqigufen.top

[Q49] 更新单行
来源：http://cpm.chenlongwang.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ctx.aibaodan.cn

[Q50] 批量更新
来源：http://wgz.yonumen.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zav.pengpengdd.cyou

[Q51] 用子查询更新
来源：http://inc.ybcxt.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ctc.haohaochexian.top

[Q52] 删除指定行
来源：http://otc.guannengcc.top

DELETE FROM users WHERE id = 10;
来源：http://jts.fehbvm.com

[Q53] 按条件删除
来源：http://vaa.yvedp.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fmy.jqgufenzy.top

[Q54] 清空表
来源：http://ucx.iojbl.cn

TRUNCATE TABLE logs;
来源：http://mbx.wangshuangyany.cn

[Q55] 排名（并列占位）
来源：http://kuq.zdqjudy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yos.shangyingyoupin.top

[Q56] 密集排名（并列不占位）
来源：http://esr.pycfn.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fxp.jinyuanbaomall.cn

[Q57] 行号
来源：http://jee.nanxinkj.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pih.cheryme.top

[Q58] 累计求和
来源：http://bxn.fengsongda.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jhb.bbcook.cn

[Q59] 分组内累计
来源：http://zke.chenzaomai.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gmn.yuxming.cn

[Q60] 取上一行 / 下一行
来源：http://wko.hnqzz.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mes.guowangkeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://znu.xylfe.cn

[Q61] 移动平均
来源：http://fnx.epnwcf.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rnq.sxryk.cn

[Q62] 分组占比
来源：http://eaq.jinghuilouyu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lzx.hesvh.cn

[Q63] 开启事务
来源：http://gxu.ppjwa.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yrn.zycfv.cn

[Q64] 提交事务
来源：http://tgm.hnqzz.top

COMMIT;
来源：http://rjs.yj202588.top

[Q65] 回滚事务
来源：http://tnc.shanyushiyangkeji.top

ROLLBACK;
来源：http://law.cashguo.top

[Q66] 行锁查询
来源：http://xhn.chenzaomai.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mqw.pengpengdd.cyou

[Q67] 设置隔离级别
来源：http://jax.0kj1m.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fnc.daxiang520.top

[Q68] 保存点
来源：http://fxn.hammf.cn

SAVEPOINT sp1;
来源：http://kun.yvedp.cn

ROLLBACK TO sp1;
来源：http://npc.xylfe.cn

[Q69] 查看执行计划
来源：http://pfa.sweek.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cxw.yuxming.cn

[Q70] 更新统计信息
来源：http://tif.zycfv.cn

ANALYZE TABLE users;
来源：http://onw.snrcjt.cn

[Q71] 查看建表语句
来源：http://blk.shuidangran.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qwt.cheryme.top

[Q72] 查看索引
来源：http://ree.vehdjk.com

SHOW INDEX FROM users;
来源：http://ymv.pengpengdd.cyou

[Q73] 查看表状态
来源：http://rnj.yj20258.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rln.uphjek.com

[Q74] 强制使用索引
来源：http://hrs.316326.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://slk.tian-w.cn

[Q75] 日期格式化
来源：http://nuh.pycfn.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sjx.smart0.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://whx.feifeiyinyue.top

[Q76] 按天统计
来源：http://rts.snrcjt.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://boc.jqgfzy.top

[Q77] 时间加减
来源：http://rpd.ppjwa.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uae.shanyushiyangkeji.top

[Q78] 当前时间
来源：http://msf.tianlin.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gwz.tanke756.top

[Q79] 字符串拼接
来源：http://ydr.nanxuanxn.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dvd.quarkkingdee.top

[Q80] 字符串截取
来源：http://zhf.svipenyu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jei.cheryme.top

[Q81] 字符串替换
来源：http://ldh.gzhubu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://reh.hnqzz.top

[Q82] 字符长度与字节长度
来源：http://ukv.redwolf501.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://npw.ydzc1.top

[Q83] 大小写转换
来源：http://dpj.epnwcf.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kvk.zhaomingkeji.xyz

[Q84] 去除首尾空格
来源：http://jie.zhiwuduotai.top

SELECT TRIM(name) FROM users;
来源：http://xnn.hesvh.cn

[Q85] 数值取整
来源：http://xvf.feifeiyinyue.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cro.sjlbkw.cn

[Q86] 读取 JSON 字段
来源：http://klq.hysaishi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qea.tianlin.xyz

[Q87] JSON 字段做条件
来源：http://xsy.havefunace.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hmp.sjlbkw.cn

[Q88] 行转列（条件聚合）
来源：http://hdn.hywenlv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yrq.fanxiaobao.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ewn.ydjk.org.cn

[Q89] 判断表是否存在
来源：http://rsk.havefunace.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uot.ywan-chungtsiang.top

[Q90] 生成序号列
来源：http://nlg.pycfn.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fin.yj20258.top

================================================================================
来源：http://lrn.xingfuxueyuan.xyz

R. Bash 专题
来源：http://wxv.shzxlz.cn

================================================================================
来源：http://tww.yongpay.top

[R01] shebang 与严格模式
来源：http://wft.daxiang520.top

#!/usr/bin/env bash
来源：http://lqc.yueranfly.top

set -euo pipefail
来源：http://sgh.0kj1m.cn

[R02] 变量赋值与使用
来源：http://wti.tian-w.cn

name="Tom"; echo "$name"
来源：http://dnb.nanxinkj.top

[R03] 只读变量
来源：http://lxl.chenjidiqi.icu

readonly PI=3.14
来源：http://avx.zhongyouzk.top

[R04] 位置参数
来源：http://vct.yvedp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://aam.sufxvd.cn

[R05] 参数默认值
来源：http://fly.hongshengwenyu.top

name="${1:-default}"
来源：http://thr.yongpay.top

[R06] 判断命令是否存在
来源：http://byj.xziqi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gwe.zhiwuduotai.top

[R07] if 判断文件
来源：http://pyp.chenlongwang.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qph.yuanzhike.top

[R08] 数值比较
来源：http://tvk.daxiang520.top

if (( a > b )); then echo "a 更大"; fi
来源：http://lwo.cheryme.top

[R09] 字符串比较
来源：http://djr.yuanzhike.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ssw.cqqwz.cn

[R10] 正则匹配
来源：http://lyn.gotoacloud.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lph.jlsjyb.cn

[R11] case 多分支
来源：http://pkw.cheryme.top

case "$1" in
来源：http://mjf.sysykeji.top

start) echo "启动" ;;
来源：http://hbv.jinghuilouyu.cn

stop)  echo "停止" ;;
来源：http://azm.jinqigfzy.top

*)     echo "未知命令" ;;
来源：http://zsj.haohaochexian.top

esac
来源：http://kpz.gzhubu.top

[R12] for 遍历文件
来源：http://obb.ctjpmb.com

for f in *.txt; do echo "$f"; done
来源：http://zmv.hongshengwenyu.top

[R13] for 计数循环
来源：http://tiv.0kj1m.cn

for i in {1..10}; do echo "$i"; done
来源：http://zyu.316326.xyz

[R14] C 风格 for
来源：http://rgx.vehdjk.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nux.ivvv.top

[R15] while 逐行读文件
来源：http://luv.cdnleiting.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mcj.wangdashe.top

[R16] until 等待条件
来源：http://hij.sufxvd.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jxr.zhijiandao.cn

[R17] 数组定义与取值
来源：http://tnm.gogol.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://blz.gaohongyu789.top

[R18] 遍历数组
来源：http://jdl.316326.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dcq.sweek.top

[R19] 数组长度
来源：http://cda.sweek.top

echo "${#arr[@]}"
来源：http://bna.nanxinkj.top

[R20] 关联数组（字典）
来源：http://tqv.cqqwz.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vun.hnxiangtu.top

[R21] 字符串长度
来源：http://djf.fktsv.cn

echo "${#s}"
来源：http://ssp.bjfxy.top

[R22] 截取子串
来源：http://yjq.yfazqb.com

echo "${s:0:5}"
来源：http://gfp.ivvv.top

[R23] 字符串替换
来源：http://tmg.xingfuxueyuan.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://czg.daria6918.cn

[R24] 大小写转换
来源：http://bvq.jinghuilouyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://brr.epnwcf.com

[R25] 去后缀 / 去前缀
来源：http://dfv.guannengcc.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://acq.cashguo.top

[R26] 命令替换
来源：http://xlo.bjfxy.top

now=$(date +%F); echo "$now"
来源：http://isk.yvedp.cn

[R27] 算术展开
来源：http://rkw.316326.xyz

echo $((1 + 2 * 3))
来源：http://urt.mhx1999.top

[R28] 浮点运算
来源：http://xbu.nanxinkj.top

echo "scale=2; 10/3" | bc
来源：http://xcn.gogol.net.cn

[R29] 定义函数
来源：http://khf.cqqwz.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wml.shanyushiyangkeji.top

[R30] 函数返回状态码
来源：http://ypv.ehwqpu.com

f() { return 0; }; f || echo "失败了"
来源：http://vfj.c1oappe.top

[R31] 局部变量
来源：http://prp.pengpengdd.cyou

f() { local x=1; echo "$x"; }
来源：http://mug.ppjwa.cn

[R32] 参数个数校验
来源：http://hss.chenzaomai.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lsp.smart0.xyz

[R33] 捕获错误并提示行号
来源：http://kob.daxiang520.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ply.cashguo.top

[R34] 退出时清理
来源：http://aoo.sjlbkw.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jwj.haohaochexian.top

[R35] 后台执行并等待
来源：http://gsw.chenzaomai.com

sleep 5 & pid=$!; wait "$pid"
来源：http://wyn.jianghu66.top

[R36] 并发执行多个任务
来源：http://byx.uphjek.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sgq.jqgfzy.top

[R37] 把输出赋给变量
来源：http://xgo.hfpthk.cn

files=$(ls -1)
来源：http://aay.redwolf501.top

[R38] 管道串联
来源：http://eui.fehbvm.com

cat a.txt | grep -i error | wc -l
来源：http://gzj.52xcode.cn

[R39] 重定向标准输出与错误
来源：http://svv.sufxvd.cn

cmd > out.log 2>&1
来源：http://xue.xinyue.icu

[R40] 追加写日志
来源：http://dah.svipenyu.cn

echo "log" >> out.log
来源：http://mbt.zhaomingkeji.xyz

[R41] 丢弃输出
来源：http://ckm.epnwcf.com

cmd >/dev/null 2>&1
来源：http://oef.xziqi.cn

[R42] 输入重定向
来源：http://gtw.xuetiantiany.cn

wc -l < a.txt
来源：http://fee.ydjk.org.cn

[R43] 按名字查找文件
来源：http://xeb.zhengqikj.top

find . -name "*.log" -type f
来源：http://spa.vqdsnc.cn

[R44] 按修改时间查找
来源：http://fch.nanxuanxn.top

find . -mtime -7 -type f
来源：http://jdw.svipenyu.cn

[R45] 批量删除
来源：http://vye.hnxiangtu.top

find . -name "*.tmp" -delete
来源：http://byn.zhoulong.xyz

[R46] 递归替换文件内容
来源：http://xkm.zycfv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uyn.ydjk.org.cn

[R47] sed 单行替换
来源：http://nue.gzhubu.top

sed -i 's/foo/bar/g' a.txt
来源：http://nbb.chenzaomai.com

[R48] awk 取指定列
来源：http://oef.sufxvd.cn

awk '{print $1, $3}' a.txt
来源：http://xwj.jinghuilouyu.cn

[R49] awk 带条件
来源：http://xti.fehbvm.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fih.snrcjt.cn

[R50] awk 求和
来源：http://tmz.zhiwuduotai.top

awk '{s += $2} END {print s}' a.txt
来源：http://vcy.xuetiantiany.cn

[R51] 排序去重取前几
来源：http://fue.zdqjudy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://mqn.hnqzz.top

[R52] 统计行数
来源：http://yuc.zhijiandao.cn

wc -l a.txt
来源：http://sud.zhengqikj.top

[R53] 查看文件头与实时尾
来源：http://gqy.jinyuanbaomall.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nvf.hammf.cn

[R54] 比较两个文件
来源：http://tmz.ybcxt.top

diff a.txt b.txt
来源：http://tyi.tarul.cn

[R55] 压缩与解压
来源：http://muc.hnqzz.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vkt.shanyushiyangkeji.top

[R56] 远程拷贝
来源：http://yse.sweek.top

scp file user@host:/path/
来源：http://vie.fanxiaobao.xyz

[R57] 远程执行命令
来源：http://har.yongpay.top

ssh user@host 'uptime'
来源：http://gdz.dashuyun.cn

[R58] 下载文件
来源：http://euc.jqgfzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xjd.andypj.xyz

[R59] 发 POST JSON
来源：http://iwb.hesvh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ttd.snrcjt.cn

[R60] 只看 HTTP 状态码
来源：http://awu.epnwcf.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ocy.epnwcf.com

[R61] 磁盘占用
来源：http://xbo.tarul.cn

df -h;  du -sh *
来源：http://mge.meibo888.top

[R62] 找最占空间的文件
来源：http://hvk.daxiang520.top

du -ah . | sort -rh | head -10
来源：http://mqa.yfazqb.com

[R63] 内存与进程
来源：http://qls.cheryme.top

free -h;  ps aux | grep nginx
来源：http://aes.havefunace.top

[R64] 结束进程
来源：http://ylp.zhixingplan.top

kill -9 $(pgrep -f app.py)
来源：http://dav.shanyushiyangtech.top

[R65] 查看端口占用
来源：http://cee.jyoumei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lxs.pengpengdd.cyou

[R66] 定时任务
来源：http://upw.bbcook.cn

crontab -e;  crontab -l
来源：http://dbh.tian-w.cn

[R67] 生成随机十六进制串
来源：http://afr.gotoacloud.top

openssl rand -hex 16
来源：http://okb.hywenlv.cn

[R68] 计算文件校验值
来源：http://gdk.nanxuanxn.top

sha256sum a.txt;  md5sum a.txt
来源：http://bqi.yuxming.cn

[R69] 生成随机密码
来源：http://zun.quarkkingdee.top

head -c 16 /dev/urandom | base64
来源：http://mby.cucudq.cn

[R70] 时间戳与互转
来源：http://akp.epnwcf.com

date +%s;  date -d @1700000000
来源：http://yre.nwbrower.top

[R71] 日期格式化
来源：http://mkm.hesvh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qyu.smart0.xyz

[R72] 等待端口就绪
来源：http://fha.hongshengwenyu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qpm.cucudq.cn

[R73] 分割大日志
来源：http://nwv.nanxuanxn.top

split -l 1000 big.log part_
来源：http://kgt.xylfe.cn

[R74] 批量重命名
来源：http://iqv.gzhubu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qly.wangdashe.top

[R75] 导出环境变量
来源：http://lpa.bbcook.cn

export PATH="$HOME/bin:$PATH"
来源：http://nsu.zhoulong.xyz

[R76] 使用临时文件
来源：http://qhf.hammf.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kir.guannengcc.top

[R77] 读取用户输入
来源：http://uzz.pengpengdd.cyou

read -rp "请输入: " ans
来源：http://cix.xuanzx.com

[R78] 交互式菜单
来源：http://kya.jlsjyb.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mmg.aizwys.cn

[R79] 解析命令行选项
来源：http://ifr.sxryk.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dnj.ppjwa.cn

[R80] 查看脚本执行耗时
来源：http://ieq.fktsv.cn

time ./run.sh
来源：http://xzn.yonumen.top

================================================================================
来源：http://lao.gotoacloud.top

S. C / C++ 专题
来源：http://ers.svipenyu.cn

================================================================================
来源：http://xhe.snrcjt.cn

[S01] C：Hello World
来源：http://nog.ybcxt.top

#include <stdio.h>
来源：http://mxx.snrcjt.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cfq.zhaomingkeji.xyz

[S02] C：变量与格式化输出
来源：http://ihg.shanyushiyangkeji.top

int a = 10; printf("%d\n", a);
来源：http://gej.hnxiangtu.top

[S03] C：读入整数
来源：http://ypb.cucudq.cn

int x; scanf("%d", &x);
来源：http://fin.hnqzz.top

[S04] C：字符串复制
来源：http://yqv.zhixingplan.top

char dst[32]; strcpy(dst, "hi");
来源：http://bay.jinqigfzy.top

[S05] C：字符串长度
来源：http://jaz.nanxuanxn.top

strlen(s)
来源：http://feu.9152youxi.cn

[S06] C：字符串比较
来源：http://hqy.tarul.cn

strcmp(a, b) == 0
来源：http://xgo.cdnleiting.top

[S07] C：数组遍历求和
来源：http://uoe.sxryk.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xjl.ivvv.top

[S08] C：动态内存分配与释放
来源：http://czz.shangyingyoupin.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uyk.meibo888.top

[S09] C：结构体定义与初始化
来源：http://vwp.shanyushiyangtech.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fpg.hcnkem.com

[S10] C：指针与解引用
来源：http://zzr.hammf.cn

int *p = &a;  *p = 5;
来源：http://axc.haohaochexian.top

[S11] C：逐行读文件
来源：http://wtk.shuidangran.top

FILE *f = fopen("a.txt", "r");
来源：http://puv.jiagoushi.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://rvo.jiagoushi.top

fclose(f);
来源：http://enu.dashuyun.cn

[S12] C：写文件
来源：http://sei.yueranfly.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://whr.ctjpmb.com

[S13] C：宏定义
来源：http://xlq.guowangkeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yep.sweek.top

[S14] C：枚举
来源：http://njk.jqgufenzy.top

enum Color { RED, GREEN, BLUE };
来源：http://lgi.0kj1m.cn

[S15] C：类型转换
来源：http://wta.snrcjt.cn

(double) a / b
来源：http://wee.yuxming.cn

[S16] C：位操作置位
来源：http://och.hammf.cn


<!-- 参考信息 -->