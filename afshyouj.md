代发 wailian999

[Q44] IN 子查询
来源：http://uts.ivvv.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ctf.xuetiantiany.cn

[Q45] EXISTS 判断存在
来源：http://bef.wangshuangyany.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sds.gaohongyu789.top

[Q46] NOT EXISTS 判断不存在
来源：http://lsv.gogol.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jkj.kuanghao11.cn

[Q47] 与平均值比较
来源：http://pfl.jinghuilouyu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tgx.vqdsnc.cn

[Q48] CTE 公用表表达式
来源：http://mfa.52xcode.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jxk.haohaochexian.top

SELECT * FROM t WHERE c > 5;
来源：http://jxt.tanke756.top

[Q49] 更新单行
来源：http://gii.sufxvd.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tyt.birdmap.top

[Q50] 批量更新
来源：http://rme.gogol.net.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yux.fehbvm.com

[Q51] 用子查询更新
来源：http://cde.yj20258888.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mda.xinyue.icu

[Q52] 删除指定行
来源：http://ofl.yfazqb.com

DELETE FROM users WHERE id = 10;
来源：http://jxs.haohaochexian.top

[Q53] 按条件删除
来源：http://pow.zhaomingkeji.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://txg.jyoumei.cn

[Q54] 清空表
来源：http://jxy.sweek.top

TRUNCATE TABLE logs;
来源：http://ncz.wangshuangyany.cn

[Q55] 排名（并列占位）
来源：http://ucw.yj20258888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ijo.daria6918.cn

[Q56] 密集排名（并列不占位）
来源：http://gfz.chenzaomai.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nxg.shanyushiyangkeji.top

[Q57] 行号
来源：http://uua.gogol.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jrv.yangfankeji.com

[Q58] 累计求和
来源：http://idh.yonumen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vto.zhiwuduotai.top

[Q59] 分组内累计
来源：http://zab.shanyushiyangkeji.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bth.yueranfly.top

[Q60] 取上一行 / 下一行
来源：http://bog.hongshengwenyu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yrj.haohaochexian.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zvw.zhaomingkeji.xyz

[Q61] 移动平均
来源：http://zdy.quarkkingdee.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nqf.ppjwa.cn

[Q62] 分组占比
来源：http://qej.xziqi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://two.xingfuxueyuan.xyz

[Q63] 开启事务
来源：http://yyk.zhaomingkeji.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://ngw.chenjidiqi.icu

[Q64] 提交事务
来源：http://clk.yueranfly.top

COMMIT;
来源：http://fwf.jiagoushi.top

[Q65] 回滚事务
来源：http://glo.xziqi.cn

ROLLBACK;
来源：http://ega.havefunace.top

[Q66] 行锁查询
来源：http://qkd.jinqigufen.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fws.fanxiaobao.xyz

[Q67] 设置隔离级别
来源：http://cyn.smart0.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hts.birdmap.top

[Q68] 保存点
来源：http://eiq.yj20258.top

SAVEPOINT sp1;
来源：http://tkt.ybcxt.top

ROLLBACK TO sp1;
来源：http://qei.shzxlz.cn

[Q69] 查看执行计划
来源：http://map.hnqzz.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zmr.sxryk.cn

[Q70] 更新统计信息
来源：http://qub.vqdsnc.cn

ANALYZE TABLE users;
来源：http://dlb.0kj1m.cn

[Q71] 查看建表语句
来源：http://qzb.zhijiandao.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qbf.yueranfly.top

[Q72] 查看索引
来源：http://hqz.zdbjq.cn

SHOW INDEX FROM users;
来源：http://jqq.jiagoushi.top

[Q73] 查看表状态
来源：http://xpu.nwbrower.top

SHOW TABLE STATUS LIKE 'users';
来源：http://qak.yj20258888.top

[Q74] 强制使用索引
来源：http://rxa.guannengcc.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nos.meibo888.top

[Q75] 日期格式化
来源：http://kvd.fanxiaobao.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mxr.yonumen.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zto.jqgufenzy.top

[Q76] 按天统计
来源：http://xfl.fehbvm.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zjz.cheryme.top

[Q77] 时间加减
来源：http://umm.hcnkem.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uti.yvedp.cn

[Q78] 当前时间
来源：http://doy.fzhhl.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gnm.jiagoushi.top

[Q79] 字符串拼接
来源：http://zsq.hnxiangtu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nfc.yvedp.cn

[Q80] 字符串截取
来源：http://iry.nanxinkj.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ssd.hywenlv.cn

[Q81] 字符串替换
来源：http://ejl.hammf.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jco.gogol.net.cn

[Q82] 字符长度与字节长度
来源：http://uwt.ybcxt.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rxr.dashuyun.cn

[Q83] 大小写转换
来源：http://spi.zhongyouzk.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://teg.yj20258888.top

[Q84] 去除首尾空格
来源：http://qhj.iojbl.cn

SELECT TRIM(name) FROM users;
来源：http://kfw.andypj.xyz

[Q85] 数值取整
来源：http://bmc.jianghu66.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bmt.daxiang520.top

[Q86] 读取 JSON 字段
来源：http://ecl.yfazqb.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://iqm.tianlin.xyz

[Q87] JSON 字段做条件
来源：http://uld.yvedp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xjz.sysykeji.top

[Q88] 行转列（条件聚合）
来源：http://pki.jinyuanbaomall.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pot.daxiang520.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://atj.sjlbkw.cn

[Q89] 判断表是否存在
来源：http://acv.ctjpmb.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wma.redwolf501.top

[Q90] 生成序号列
来源：http://apx.yangfankeji.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zhr.andypj.xyz

================================================================================
来源：http://bzd.xuetiantiany.cn

R. Bash 专题
来源：http://bfy.yueranfly.top

================================================================================
来源：http://ely.hnqzz.top

[R01] shebang 与严格模式
来源：http://ojy.jinqigufen.top

#!/usr/bin/env bash
来源：http://cjk.uphjek.com

set -euo pipefail
来源：http://ywu.uphjek.com

[R02] 变量赋值与使用
来源：http://equ.tanke756.top

name="Tom"; echo "$name"
来源：http://bmz.ivvv.top

[R03] 只读变量
来源：http://nop.zhixingplan.top

readonly PI=3.14
来源：http://fec.yuxming.cn

[R04] 位置参数
来源：http://rgw.xuanzx.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tlg.uphjek.com

[R05] 参数默认值
来源：http://fsa.shanyushiyangtech.top

name="${1:-default}"
来源：http://ayc.jianghu66.top

[R06] 判断命令是否存在
来源：http://fjl.zycfv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sss.aibaodan.cn

[R07] if 判断文件
来源：http://lmk.tian-w.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mqf.0kj1m.cn

[R08] 数值比较
来源：http://hsl.hongshengwenyu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://cyz.andypj.xyz

[R09] 字符串比较
来源：http://uwn.shanyushiyangtech.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://art.shzxlz.cn

[R10] 正则匹配
来源：http://dvd.fehbvm.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pde.shanyushiyangtech.top

[R11] case 多分支
来源：http://aeh.jinqigfzy.top

case "$1" in
来源：http://xwl.fanxiaobao.xyz

start) echo "启动" ;;
来源：http://yhv.daxiang520.top

stop)  echo "停止" ;;
来源：http://zcw.fanxiaobao.xyz

*)     echo "未知命令" ;;
来源：http://gmf.yueranfly.top

esac
来源：http://vyg.jqgufenzy.top

[R12] for 遍历文件
来源：http://cwl.tian-w.cn

for f in *.txt; do echo "$f"; done
来源：http://pgi.hnqzz.top

[R13] for 计数循环
来源：http://wij.jlsjyb.cn

for i in {1..10}; do echo "$i"; done
来源：http://phk.meibo888.top

[R14] C 风格 for
来源：http://oix.fktsv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ccy.xylfe.cn

[R15] while 逐行读文件
来源：http://wwu.meibo888.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ltw.smart0.xyz

[R16] until 等待条件
来源：http://bye.dashuyun.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fkm.wangshuangyany.cn

[R17] 数组定义与取值
来源：http://pni.316326.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://qwd.birdmap.top

[R18] 遍历数组
来源：http://coe.yuanzhike.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://idb.bjfxy.top

[R19] 数组长度
来源：http://tos.yanxiufei.cn

echo "${#arr[@]}"
来源：http://gjb.cheryme.top

[R20] 关联数组（字典）
来源：http://hyl.daxiang520.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wrt.aibaodan.cn

[R21] 字符串长度
来源：http://lzn.redwolf501.top

echo "${#s}"
来源：http://all.chenlongwang.top

[R22] 截取子串
来源：http://cyu.aibaodan.cn

echo "${s:0:5}"
来源：http://daw.sxryk.cn

[R23] 字符串替换
来源：http://zbi.zhixingplan.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kiu.vehdjk.com

[R24] 大小写转换
来源：http://zlx.bbcook.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ssv.wangshuangyany.cn

[R25] 去后缀 / 去前缀
来源：http://fpd.jqgufenzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://yze.52xcode.cn

[R26] 命令替换
来源：http://mwd.shuidangran.top

now=$(date +%F); echo "$now"
来源：http://kds.pengpengdd.cyou

[R27] 算术展开
来源：http://rax.sufxvd.cn

echo $((1 + 2 * 3))
来源：http://qvu.ppjwa.cn

[R28] 浮点运算
来源：http://ydr.shzxlz.cn

echo "scale=2; 10/3" | bc
来源：http://gqv.haohaochexian.top

[R29] 定义函数
来源：http://jls.smart0.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ifa.zdbjq.cn

[R30] 函数返回状态码
来源：http://fiq.haohaochexian.top

f() { return 0; }; f || echo "失败了"
来源：http://zqg.yj20258888.top

[R31] 局部变量
来源：http://nmd.9152youxi.cn

f() { local x=1; echo "$x"; }
来源：http://wcy.jlsjyb.cn

[R32] 参数个数校验
来源：http://aac.yvedp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fwc.vqdsnc.cn

[R33] 捕获错误并提示行号
来源：http://qid.zhengqikj.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jsd.zdbjq.cn

[R34] 退出时清理
来源：http://slk.zhaomingkeji.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://eiz.jqgfzy.top

[R35] 后台执行并等待
来源：http://wsq.jyoumei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gby.redwolf501.top

[R36] 并发执行多个任务
来源：http://rvb.yongpay.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ahn.jqgufenzy.top

[R37] 把输出赋给变量
来源：http://hit.pycfn.com

files=$(ls -1)
来源：http://vka.meibo888.top

[R38] 管道串联
来源：http://bgl.52xcode.cn

cat a.txt | grep -i error | wc -l
来源：http://cuz.chenzaomai.com

[R39] 重定向标准输出与错误
来源：http://zkw.yvedp.cn

cmd > out.log 2>&1
来源：http://mnn.ehwqpu.com

[R40] 追加写日志
来源：http://ffs.yongpay.top

echo "log" >> out.log
来源：http://gcv.sysykeji.top

[R41] 丢弃输出
来源：http://mxp.ywan-chungtsiang.top

cmd >/dev/null 2>&1
来源：http://ttt.dianchejie.cn

[R42] 输入重定向
来源：http://pwo.meibo888.top

wc -l < a.txt
来源：http://jjv.feifeiyinyue.top

[R43] 按名字查找文件
来源：http://faw.316326.xyz

find . -name "*.log" -type f
来源：http://kbr.nwbrower.top

[R44] 按修改时间查找
来源：http://adu.jiagoushi.top

find . -mtime -7 -type f
来源：http://ysz.zhijiandao.cn

[R45] 批量删除
来源：http://jbp.sysykeji.top

find . -name "*.tmp" -delete
来源：http://pet.fzhhl.top

[R46] 递归替换文件内容
来源：http://ltv.zhaomingkeji.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dto.gogol.net.cn

[R47] sed 单行替换
来源：http://mzw.hnxiangtu.top

sed -i 's/foo/bar/g' a.txt
来源：http://azu.hysaishi.cn

[R48] awk 取指定列
来源：http://cit.hysaishi.cn

awk '{print $1, $3}' a.txt
来源：http://pcb.pengpengdd.cyou

[R49] awk 带条件
来源：http://wei.fanxiaobao.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bzy.cdnleiting.top

[R50] awk 求和
来源：http://kzj.0kj1m.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bpg.yfazqb.com

[R51] 排序去重取前几
来源：http://adz.fktsv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tph.gzhubu.top

[R52] 统计行数
来源：http://dtl.yueranfly.top

wc -l a.txt
来源：http://nvp.zdbjq.cn

[R53] 查看文件头与实时尾
来源：http://kss.hysaishi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gcw.hnxiangtu.top

[R54] 比较两个文件
来源：http://bhy.zhixingplan.top

diff a.txt b.txt
来源：http://hxx.pycfn.com

[R55] 压缩与解压
来源：http://ayb.zhoulong.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://igo.tian-w.cn

[R56] 远程拷贝
来源：http://rjx.shangyingyoupin.top

scp file user@host:/path/
来源：http://gki.xuanzx.com

[R57] 远程执行命令
来源：http://hjm.jinqigfzy.top

ssh user@host 'uptime'
来源：http://hca.chenzaomai.com

[R58] 下载文件
来源：http://odw.hammf.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://njw.yj20258888.top

[R59] 发 POST JSON
来源：http://dsq.fktsv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vcz.pycfn.com

[R60] 只看 HTTP 状态码
来源：http://gxw.aizwys.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ofc.chenjidiqi.icu

[R61] 磁盘占用
来源：http://oyt.jinghuilouyu.cn

df -h;  du -sh *
来源：http://kum.yangfankeji.com

[R62] 找最占空间的文件
来源：http://bxd.yonumen.top

du -ah . | sort -rh | head -10
来源：http://dov.cdnleiting.top

[R63] 内存与进程
来源：http://hbk.wangshuangyany.cn

free -h;  ps aux | grep nginx
来源：http://jjn.zhoulong.xyz

[R64] 结束进程
来源：http://pdq.haohaochexian.top

kill -9 $(pgrep -f app.py)
来源：http://riw.sjlbkw.cn

[R65] 查看端口占用
来源：http://lkw.chenjidiqi.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wxm.hongshengwenyu.top

[R66] 定时任务
来源：http://syp.havefunace.top

crontab -e;  crontab -l
来源：http://vga.zdbjq.cn

[R67] 生成随机十六进制串
来源：http://vux.jiagoushi.top

openssl rand -hex 16
来源：http://onz.haohaochexian.top

[R68] 计算文件校验值
来源：http://bac.dianchejie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://anc.jqgfzy.top

[R69] 生成随机密码
来源：http://xqc.zhongyouzk.top

head -c 16 /dev/urandom | base64
来源：http://ccw.havefunace.top

[R70] 时间戳与互转
来源：http://cxq.zhiwuduotai.top

date +%s;  date -d @1700000000
来源：http://vir.sufxvd.cn

[R71] 日期格式化
来源：http://nye.c1oappe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://wgy.fehbvm.com

[R72] 等待端口就绪
来源：http://img.52xcode.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://clq.zhaomingkeji.xyz

[R73] 分割大日志
来源：http://zpk.ctjpmb.com

split -l 1000 big.log part_
来源：http://vku.havefunace.top

[R74] 批量重命名
来源：http://oga.vqdsnc.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fpm.shanyushiyangtech.top

[R75] 导出环境变量
来源：http://iyk.chenzaomai.com

export PATH="$HOME/bin:$PATH"
来源：http://vgg.9152youxi.cn

[R76] 使用临时文件
来源：http://ydr.cqqwz.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://igm.yvedp.cn

[R77] 读取用户输入
来源：http://iex.ybcxt.top

read -rp "请输入: " ans
来源：http://ayh.9152youxi.cn

[R78] 交互式菜单
来源：http://noc.aibaodan.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ajk.xingfuxueyuan.xyz

[R79] 解析命令行选项
来源：http://efp.sufxvd.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ybx.zdbjq.cn

[R80] 查看脚本执行耗时
来源：http://mlf.fzhhl.top

time ./run.sh
来源：http://waf.zycfv.cn

================================================================================
来源：http://hbs.chenjidiqi.icu

S. C / C++ 专题
来源：http://lnv.jqgfzy.top

================================================================================
来源：http://xqq.fengsongda.top

[S01] C：Hello World
来源：http://lfu.nwbrower.top

#include <stdio.h>
来源：http://leb.ehwqpu.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://xcc.xingfuxueyuan.xyz

[S02] C：变量与格式化输出
来源：http://zen.dianchejie.cn

int a = 10; printf("%d\n", a);
来源：http://czr.sufxvd.cn

[S03] C：读入整数
来源：http://skq.wangshuangyany.cn

int x; scanf("%d", &x);
来源：http://tif.cqqwz.cn

[S04] C：字符串复制
来源：http://nnh.hysaishi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xlw.yuxming.cn

[S05] C：字符串长度
来源：http://lqi.zhiwuduotai.top

strlen(s)
来源：http://yxd.ywan-chungtsiang.top

[S06] C：字符串比较
来源：http://pfa.haohaochexian.top

strcmp(a, b) == 0
来源：http://dqy.shanyushiyangkeji.top

[S07] C：数组遍历求和
来源：http://tct.zdqjudy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fyt.zhengqikj.top

[S08] C：动态内存分配与释放
来源：http://oub.xingfuxueyuan.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tee.zhoulong.xyz

[S09] C：结构体定义与初始化
来源：http://btp.52xcode.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sxz.feifeiyinyue.top

[S10] C：指针与解引用
来源：http://puh.xylfe.cn

int *p = &a;  *p = 5;
来源：http://boy.yfazqb.com

[S11] C：逐行读文件
来源：http://gfi.aibaodan.cn

FILE *f = fopen("a.txt", "r");
来源：http://wed.nanxinkj.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qvb.hammf.cn

fclose(f);
来源：http://gav.pycfn.com

[S12] C：写文件
来源：http://nbb.meibo888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ovk.fktsv.cn

[S13] C：宏定义
来源：http://fhf.quarkkingdee.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yhe.tanke756.top

[S14] C：枚举
来源：http://mss.hesvh.cn


<!-- 参考信息 -->