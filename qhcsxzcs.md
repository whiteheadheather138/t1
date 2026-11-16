代发 wailian999

[Q48] CTE 公用表表达式
来源：http://adc.hysaishi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vrj.aizwys.cn

SELECT * FROM t WHERE c > 5;
来源：http://psf.jinyuanbaomall.cn

[Q49] 更新单行
来源：http://thq.aizwys.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ius.hywenlv.cn

[Q50] 批量更新
来源：http://eyt.tian-w.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pkj.pycfn.com

[Q51] 用子查询更新
来源：http://zhf.tian-w.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tdh.uphjek.com

[Q52] 删除指定行
来源：http://pbv.cheryme.top

DELETE FROM users WHERE id = 10;
来源：http://neb.xuanzx.com

[Q53] 按条件删除
来源：http://lxt.redwolf501.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://iyt.feifeiyinyue.top

[Q54] 清空表
来源：http://lcw.shuidangran.top

TRUNCATE TABLE logs;
来源：http://zde.ctjpmb.com

[Q55] 排名（并列占位）
来源：http://iml.jinqigfzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tsz.fehbvm.com

[Q56] 密集排名（并列不占位）
来源：http://wxz.ppjwa.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://guy.zhaomingkeji.xyz

[Q57] 行号
来源：http://yzl.smart0.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nwh.wangdashe.top

[Q58] 累计求和
来源：http://oup.yuanzhike.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://trv.shanyushiyangkeji.top

[Q59] 分组内累计
来源：http://rki.yj20258888.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rit.zhijiandao.cn

[Q60] 取上一行 / 下一行
来源：http://cld.tian-w.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wyy.xylfe.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://npu.jinyuanbaomall.cn

[Q61] 移动平均
来源：http://mll.sweek.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rev.yuanzhike.top

[Q62] 分组占比
来源：http://kka.tanke756.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dgy.vehdjk.com

[Q63] 开启事务
来源：http://nuw.yangfankeji.com

START TRANSACTION;                -- 或 BEGIN
来源：http://lmh.hnxiangtu.top

[Q64] 提交事务
来源：http://acl.svipenyu.cn

COMMIT;
来源：http://vxb.zycfv.cn

[Q65] 回滚事务
来源：http://sfk.ywan-chungtsiang.top

ROLLBACK;
来源：http://qyb.xinyue.icu

[Q66] 行锁查询
来源：http://iig.chenjidiqi.icu

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pyz.iojbl.cn

[Q67] 设置隔离级别
来源：http://xie.pycfn.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://eyv.andypj.xyz

[Q68] 保存点
来源：http://mij.cdnleiting.top

SAVEPOINT sp1;
来源：http://wnc.gotoacloud.top

ROLLBACK TO sp1;
来源：http://rcv.quarkkingdee.top

[Q69] 查看执行计划
来源：http://ikv.yangfankeji.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wmz.sjlbkw.cn

[Q70] 更新统计信息
来源：http://dxn.dashuyun.cn

ANALYZE TABLE users;
来源：http://seo.shanyushiyangtech.top

[Q71] 查看建表语句
来源：http://fel.pengpengdd.cyou

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pjr.yuxming.cn

[Q72] 查看索引
来源：http://kvb.yvedp.cn

SHOW INDEX FROM users;
来源：http://pkd.fktsv.cn

[Q73] 查看表状态
来源：http://glp.jiagoushi.top

SHOW TABLE STATUS LIKE 'users';
来源：http://zfd.jyoumei.cn

[Q74] 强制使用索引
来源：http://fbl.xuanzx.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qsf.fanxiaobao.xyz

[Q75] 日期格式化
来源：http://rld.yj20258888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zxg.zdqjudy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://moq.cucudq.cn

[Q76] 按天统计
来源：http://tkw.chenzaomai.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jvk.jlsjyb.cn

[Q77] 时间加减
来源：http://rsh.hnxiangtu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yrx.zhiwuduotai.top

[Q78] 当前时间
来源：http://gng.vqdsnc.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://aeu.hammf.cn

[Q79] 字符串拼接
来源：http://bln.xinyue.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xqx.gotoacloud.top

[Q80] 字符串截取
来源：http://qea.xuetiantiany.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://krj.jiagoushi.top

[Q81] 字符串替换
来源：http://afw.snrcjt.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lnd.jinqigfzy.top

[Q82] 字符长度与字节长度
来源：http://qou.fzhhl.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rmo.kuanghao11.cn

[Q83] 大小写转换
来源：http://ldj.pycfn.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://adi.gotoacloud.top

[Q84] 去除首尾空格
来源：http://aen.ydzc1.top

SELECT TRIM(name) FROM users;
来源：http://epq.shanyushiyangtech.top

[Q85] 数值取整
来源：http://rzt.hesvh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://utj.9152youxi.cn

[Q86] 读取 JSON 字段
来源：http://gnw.tarul.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://eyc.vehdjk.com

[Q87] JSON 字段做条件
来源：http://xbf.vehdjk.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://enm.xuetiantiany.cn

[Q88] 行转列（条件聚合）
来源：http://jnc.jinqigufen.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dzp.xylfe.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ber.andypj.xyz

[Q89] 判断表是否存在
来源：http://taa.yj20258.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pvl.sysykeji.top

[Q90] 生成序号列
来源：http://zpv.316326.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xag.bjfxy.top

================================================================================
来源：http://zgu.andypj.xyz

R. Bash 专题
来源：http://foe.shangyingyoupin.top

================================================================================
来源：http://dlg.shzxlz.cn

[R01] shebang 与严格模式
来源：http://xnr.vehdjk.com

#!/usr/bin/env bash
来源：http://wpn.sysykeji.top

set -euo pipefail
来源：http://pvh.yuxming.cn

[R02] 变量赋值与使用
来源：http://sic.yonumen.top

name="Tom"; echo "$name"
来源：http://zzx.fengsongda.top

[R03] 只读变量
来源：http://mmz.ydzc1.top

readonly PI=3.14
来源：http://iiq.jinghuilouyu.cn

[R04] 位置参数
来源：http://fjz.dashuyun.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mov.zhengqikj.top

[R05] 参数默认值
来源：http://kot.hywenlv.cn

name="${1:-default}"
来源：http://oqz.zhixingplan.top

[R06] 判断命令是否存在
来源：http://jmw.cashguo.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bfp.shanyushiyangkeji.top

[R07] if 判断文件
来源：http://wfm.shangyingyoupin.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xlo.hnqzz.top

[R08] 数值比较
来源：http://tut.shanyushiyangtech.top

if (( a > b )); then echo "a 更大"; fi
来源：http://juz.yuanzhike.top

[R09] 字符串比较
来源：http://dlz.ywan-chungtsiang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mnb.chenzaomai.com

[R10] 正则匹配
来源：http://wws.jinghuilouyu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vdv.0kj1m.cn

[R11] case 多分支
来源：http://ejn.shanyushiyangkeji.top

case "$1" in
来源：http://tzb.hfpthk.cn

start) echo "启动" ;;
来源：http://opr.xziqi.cn

stop)  echo "停止" ;;
来源：http://sps.ywan-chungtsiang.top

*)     echo "未知命令" ;;
来源：http://bnk.ybcxt.top

esac
来源：http://otu.svipenyu.cn

[R12] for 遍历文件
来源：http://jjn.wangdashe.top

for f in *.txt; do echo "$f"; done
来源：http://ejn.xingfuxueyuan.xyz

[R13] for 计数循环
来源：http://ezl.0kj1m.cn

for i in {1..10}; do echo "$i"; done
来源：http://oea.gzhubu.top

[R14] C 风格 for
来源：http://qru.shuidangran.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://aez.snrcjt.cn

[R15] while 逐行读文件
来源：http://whv.havefunace.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://him.guowangkeji.top

[R16] until 等待条件
来源：http://qqc.havefunace.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hje.feifeiyinyue.top

[R17] 数组定义与取值
来源：http://nka.xziqi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://eag.cucudq.cn

[R18] 遍历数组
来源：http://bob.birdmap.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yig.dashuyun.cn

[R19] 数组长度
来源：http://knr.xylfe.cn

echo "${#arr[@]}"
来源：http://pcy.bbcook.cn

[R20] 关联数组（字典）
来源：http://zar.zhongyouzk.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kym.gogol.net.cn

[R21] 字符串长度
来源：http://rkc.yj20258888.top

echo "${#s}"
来源：http://ysj.vqdsnc.cn

[R22] 截取子串
来源：http://ind.shuidangran.top

echo "${s:0:5}"
来源：http://amn.zhixingplan.top

[R23] 字符串替换
来源：http://hra.haohaochexian.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iph.vehdjk.com

[R24] 大小写转换
来源：http://qbe.gzhubu.top

echo "${s^^}"; echo "${s,,}"
来源：http://hrl.daria6918.cn

[R25] 去后缀 / 去前缀
来源：http://uyd.hesvh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fbt.xuanzx.com

[R26] 命令替换
来源：http://obv.jinghuilouyu.cn

now=$(date +%F); echo "$now"
来源：http://sdc.ehwqpu.com

[R27] 算术展开
来源：http://znd.yueranfly.top

echo $((1 + 2 * 3))
来源：http://lqe.yanxiufei.cn

[R28] 浮点运算
来源：http://lwg.cucudq.cn

echo "scale=2; 10/3" | bc
来源：http://yqx.dianchejie.cn

[R29] 定义函数
来源：http://pol.yangfankeji.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bat.ywan-chungtsiang.top

[R30] 函数返回状态码
来源：http://gus.sysykeji.top

f() { return 0; }; f || echo "失败了"
来源：http://lfk.haohaochexian.top

[R31] 局部变量
来源：http://oef.jinqigfzy.top

f() { local x=1; echo "$x"; }
来源：http://pdu.andypj.xyz

[R32] 参数个数校验
来源：http://ohf.gogol.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zxb.zhoulong.xyz

[R33] 捕获错误并提示行号
来源：http://rso.aizwys.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tou.fengsongda.top

[R34] 退出时清理
来源：http://xuk.yongpay.top

trap 'rm -f "$tmp"' EXIT
来源：http://wdr.jinqigufen.top

[R35] 后台执行并等待
来源：http://mdc.havefunace.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ppb.chenlongwang.top

[R36] 并发执行多个任务
来源：http://qhq.daxiang520.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dva.snrcjt.cn

[R37] 把输出赋给变量
来源：http://mdu.cucudq.cn

files=$(ls -1)
来源：http://buc.jiagoushi.top

[R38] 管道串联
来源：http://koa.iojbl.cn

cat a.txt | grep -i error | wc -l
来源：http://ngm.sxryk.cn

[R39] 重定向标准输出与错误
来源：http://xsc.zhixingplan.top

cmd > out.log 2>&1
来源：http://fiy.redwolf501.top

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz

echo "log" >> out.log
来源：http://lse.jlsjyb.cn

[R41] 丢弃输出
来源：http://alb.xuetiantiany.cn

cmd >/dev/null 2>&1
来源：http://vvt.yanxiufei.cn

[R42] 输入重定向
来源：http://ect.hysaishi.cn

wc -l < a.txt
来源：http://lyd.vqdsnc.cn

[R43] 按名字查找文件
来源：http://qhw.yongpay.top

find . -name "*.log" -type f
来源：http://ycj.birdmap.top

[R44] 按修改时间查找
来源：http://xdh.gzhubu.top

find . -mtime -7 -type f
来源：http://pvh.yueranfly.top

[R45] 批量删除
来源：http://uyl.jyoumei.cn

find . -name "*.tmp" -delete
来源：http://wsa.aizwys.cn

[R46] 递归替换文件内容
来源：http://xrl.ydjk.org.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wmz.zhixingplan.top

[R47] sed 单行替换
来源：http://hrk.nanxuanxn.top

sed -i 's/foo/bar/g' a.txt
来源：http://ahr.xylfe.cn

[R48] awk 取指定列
来源：http://uga.hysaishi.cn

awk '{print $1, $3}' a.txt
来源：http://mtg.zdbjq.cn

[R49] awk 带条件
来源：http://tav.hfpthk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://emi.ybcxt.top

[R50] awk 求和
来源：http://ezx.nwbrower.top

awk '{s += $2} END {print s}' a.txt
来源：http://nph.yangfankeji.com

[R51] 排序去重取前几
来源：http://nbx.shangyingyoupin.top

sort a.txt | uniq -c | sort -rn | head
来源：http://mev.svipenyu.cn

[R52] 统计行数
来源：http://sjk.jinqigufen.top

wc -l a.txt
来源：http://jvq.shuidangran.top

[R53] 查看文件头与实时尾
来源：http://xia.ywan-chungtsiang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://koc.wangshuangyany.cn

[R54] 比较两个文件
来源：http://nec.zhongyouzk.top

diff a.txt b.txt
来源：http://wtb.dashuyun.cn

[R55] 压缩与解压
来源：http://lgg.jyoumei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ghq.yonumen.top

[R56] 远程拷贝
来源：http://dtf.sxryk.cn

scp file user@host:/path/
来源：http://ush.jianghu66.top

[R57] 远程执行命令
来源：http://uxs.c1oappe.top

ssh user@host 'uptime'
来源：http://xhi.zycfv.cn

[R58] 下载文件
来源：http://lgl.fehbvm.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pfn.yj20258888.top

[R59] 发 POST JSON
来源：http://mui.cdnleiting.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ulq.hongshengwenyu.top

[R60] 只看 HTTP 状态码
来源：http://spb.yongpay.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xbk.hammf.cn

[R61] 磁盘占用
来源：http://biq.hesvh.cn

df -h;  du -sh *
来源：http://dlf.bbcook.cn

[R62] 找最占空间的文件
来源：http://aqk.daxiang520.top

du -ah . | sort -rh | head -10
来源：http://tlb.zhiwuduotai.top

[R63] 内存与进程
来源：http://ulu.pengpengdd.cyou

free -h;  ps aux | grep nginx
来源：http://vzj.zdqjudy.top

[R64] 结束进程
来源：http://wvk.yfazqb.com

kill -9 $(pgrep -f app.py)
来源：http://gyf.iojbl.cn

[R65] 查看端口占用
来源：http://sxi.jqgufenzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gpa.yuxming.cn

[R66] 定时任务
来源：http://cmb.daxiang520.top

crontab -e;  crontab -l
来源：http://zwh.guowangkeji.top

[R67] 生成随机十六进制串
来源：http://gxv.daria6918.cn

openssl rand -hex 16
来源：http://gvb.zhixingplan.top

[R68] 计算文件校验值
来源：http://vzc.shzxlz.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gmq.c1oappe.top

[R69] 生成随机密码
来源：http://jnh.bjfxy.top

head -c 16 /dev/urandom | base64
来源：http://lbk.jlsjyb.cn

[R70] 时间戳与互转
来源：http://gig.shanyushiyangtech.top

date +%s;  date -d @1700000000
来源：http://rsy.zhongyouzk.top

[R71] 日期格式化
来源：http://adb.hcnkem.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://ccs.xziqi.cn

[R72] 等待端口就绪
来源：http://hta.yj20258.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ufm.zdbjq.cn

[R73] 分割大日志
来源：http://oum.zhengqikj.top

split -l 1000 big.log part_
来源：http://lpl.wangdashe.top

[R74] 批量重命名
来源：http://lxm.tianlin.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lqc.sweek.top

[R75] 导出环境变量
来源：http://bjb.guannengcc.top

export PATH="$HOME/bin:$PATH"
来源：http://rsn.hongshengwenyu.top

[R76] 使用临时文件
来源：http://unq.fanxiaobao.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://njf.vqdsnc.cn

[R77] 读取用户输入
来源：http://ctv.shanyushiyangtech.top

read -rp "请输入: " ans
来源：http://flv.shanyushiyangtech.top

[R78] 交互式菜单
来源：http://amo.yangfankeji.com

select opt in a b c; do echo "$opt"; break; done
来源：http://cma.feifeiyinyue.top

[R79] 解析命令行选项
来源：http://tgg.yonumen.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yim.shanyushiyangkeji.top

[R80] 查看脚本执行耗时
来源：http://guf.hammf.cn

time ./run.sh
来源：http://gfn.ydzc1.top

================================================================================
来源：http://iwp.ctjpmb.com

S. C / C++ 专题
来源：http://uze.fengsongda.top

================================================================================
来源：http://qxi.tarul.cn

[S01] C：Hello World
来源：http://nkh.epnwcf.com

#include <stdio.h>
来源：http://jdo.meibo888.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ivu.epnwcf.com

[S02] C：变量与格式化输出
来源：http://kck.hammf.cn

int a = 10; printf("%d\n", a);
来源：http://qcp.9152youxi.cn

[S03] C：读入整数
来源：http://cob.tanke756.top

int x; scanf("%d", &x);
来源：http://ffr.sxryk.cn

[S04] C：字符串复制
来源：http://irr.zhengqikj.top

char dst[32]; strcpy(dst, "hi");
来源：http://lhy.yj20258.top

[S05] C：字符串长度
来源：http://jyl.zhaomingkeji.xyz

strlen(s)
来源：http://cdi.uphjek.com

[S06] C：字符串比较
来源：http://feb.ppjwa.cn

strcmp(a, b) == 0
来源：http://yuf.ydjk.org.cn

[S07] C：数组遍历求和
来源：http://yeg.nanxinkj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://znf.zhongyouzk.top

[S08] C：动态内存分配与释放
来源：http://cdc.hfpthk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://icg.jlsjyb.cn

[S09] C：结构体定义与初始化
来源：http://hub.fengsongda.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ncz.yuxming.cn

[S10] C：指针与解引用
来源：http://arn.zhijiandao.cn

int *p = &a;  *p = 5;
来源：http://cqr.tanke756.top

[S11] C：逐行读文件
来源：http://nta.sufxvd.cn

FILE *f = fopen("a.txt", "r");
来源：http://ukz.jianghu66.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qxe.sysykeji.top

fclose(f);
来源：http://eru.yongpay.top

[S12] C：写文件
来源：http://and.shangyingyoupin.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://usq.chenlongwang.top

[S13] C：宏定义
来源：http://vuk.hammf.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gel.vehdjk.com

[S14] C：枚举
来源：http://zbw.uphjek.com

enum Color { RED, GREEN, BLUE };
来源：http://ikj.epnwcf.com

[S15] C：类型转换
来源：http://yjs.shangyingyoupin.top

(double) a / b
来源：http://saa.feifeiyinyue.top

[S16] C：位操作置位
来源：http://xhi.fehbvm.com

x |= (1 << 3);
来源：http://mkt.jqgfzy.top

[S17] C：安全拼接字符串
来源：http://izu.cashguo.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qul.jinqigufen.top

[S18] C：命令行参数
来源：http://vsa.yvedp.cn


<!-- 参考信息 -->