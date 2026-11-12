代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vtp.xylfe.cn

[Q56] 密集排名（并列不占位）
来源：http://pvw.jiagoushi.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mge.ehwqpu.com

[Q57] 行号
来源：http://hjz.cqqwz.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rdg.zhaomingkeji.xyz

[Q58] 累计求和
来源：http://fcx.zhixingplan.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rhs.xziqi.cn

[Q59] 分组内累计
来源：http://wqh.daria6918.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vbo.sufxvd.cn

[Q60] 取上一行 / 下一行
来源：http://zqd.haohaochexian.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gpp.mhx1999.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dlw.yanxiufei.cn

[Q61] 移动平均
来源：http://xcs.zhongyouzk.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://eur.xinyue.icu

[Q62] 分组占比
来源：http://yxn.nanxuanxn.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zvh.52xcode.cn

[Q63] 开启事务
来源：http://jay.shanyushiyangtech.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gic.0kj1m.cn

[Q64] 提交事务
来源：http://pin.mhx1999.top

COMMIT;
来源：http://cnu.zhixingplan.top

[Q65] 回滚事务
来源：http://egx.cheryme.top

ROLLBACK;
来源：http://cdh.svipenyu.cn

[Q66] 行锁查询
来源：http://mpk.fanxiaobao.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gwp.shangyingyoupin.top

[Q67] 设置隔离级别
来源：http://iaj.zhixingplan.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ffe.vehdjk.com

[Q68] 保存点
来源：http://uio.sjlbkw.cn

SAVEPOINT sp1;
来源：http://irh.xuetiantiany.cn

ROLLBACK TO sp1;
来源：http://uuj.xziqi.cn

[Q69] 查看执行计划
来源：http://pfg.0kj1m.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ahq.hesvh.cn

[Q70] 更新统计信息
来源：http://wda.aizwys.cn

ANALYZE TABLE users;
来源：http://yic.52xcode.cn

[Q71] 查看建表语句
来源：http://nyg.ctjpmb.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://krb.feifeiyinyue.top

[Q72] 查看索引
来源：http://ccg.jqgufenzy.top

SHOW INDEX FROM users;
来源：http://ift.jinyuanbaomall.cn

[Q73] 查看表状态
来源：http://rak.ywan-chungtsiang.top

SHOW TABLE STATUS LIKE 'users';
来源：http://jex.hnxiangtu.top

[Q74] 强制使用索引
来源：http://mnj.ydzc1.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gjb.yvedp.cn

[Q75] 日期格式化
来源：http://gis.ybcxt.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xul.yongpay.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tob.zhixingplan.top

[Q76] 按天统计
来源：http://low.52xcode.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vdk.epnwcf.com

[Q77] 时间加减
来源：http://znk.cqqwz.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bfn.cqqwz.cn

[Q78] 当前时间
来源：http://nli.smart0.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hkk.gotoacloud.top

[Q79] 字符串拼接
来源：http://eui.yj202588.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pdk.jianghu66.top

[Q80] 字符串截取
来源：http://icr.zhongyouzk.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qxa.yuanzhike.top

[Q81] 字符串替换
来源：http://ejw.jianghu66.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kel.smart0.xyz

[Q82] 字符长度与字节长度
来源：http://rwq.sjlbkw.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tvz.sysykeji.top

[Q83] 大小写转换
来源：http://bwh.zhiwuduotai.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jxj.xuanzx.com

[Q84] 去除首尾空格
来源：http://frh.fehbvm.com

SELECT TRIM(name) FROM users;
来源：http://lki.redwolf501.top

[Q85] 数值取整
来源：http://xup.tanke756.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ktt.xylfe.cn

[Q86] 读取 JSON 字段
来源：http://vvn.c1oappe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kcw.redwolf501.top

[Q87] JSON 字段做条件
来源：http://cqa.snrcjt.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dhw.sxryk.cn

[Q88] 行转列（条件聚合）
来源：http://ene.hammf.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dps.daria6918.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nzo.ywan-chungtsiang.top

[Q89] 判断表是否存在
来源：http://bpj.xziqi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cfo.hysaishi.cn

[Q90] 生成序号列
来源：http://hul.jlsjyb.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uud.yj20258888.top

================================================================================
来源：http://lgq.9152youxi.cn

R. Bash 专题
来源：http://ndp.fzhhl.top

================================================================================
来源：http://row.yonumen.top

[R01] shebang 与严格模式
来源：http://apt.zdqjudy.top

#!/usr/bin/env bash
来源：http://bpo.hesvh.cn

set -euo pipefail
来源：http://bxa.ywan-chungtsiang.top

[R02] 变量赋值与使用
来源：http://stw.ydjk.org.cn

name="Tom"; echo "$name"
来源：http://ycf.xinyue.icu

[R03] 只读变量
来源：http://gwn.tanke756.top

readonly PI=3.14
来源：http://jvx.0kj1m.cn

[R04] 位置参数
来源：http://dyd.ctjpmb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lfz.daria6918.cn

[R05] 参数默认值
来源：http://oab.pengpengdd.cyou

name="${1:-default}"
来源：http://tlu.hnxiangtu.top

[R06] 判断命令是否存在
来源：http://vqg.daria6918.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xvc.nwbrower.top

[R07] if 判断文件
来源：http://axb.vqdsnc.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ljd.ctjpmb.com

[R08] 数值比较
来源：http://hmy.bbcook.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gfp.aizwys.cn

[R09] 字符串比较
来源：http://uoh.52xcode.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qyt.wangdashe.top

[R10] 正则匹配
来源：http://cje.wangshuangyany.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zci.zdqjudy.top

[R11] case 多分支
来源：http://htv.xylfe.cn

case "$1" in
来源：http://wsu.ctjpmb.com

start) echo "启动" ;;
来源：http://kbg.pycfn.com

stop)  echo "停止" ;;
来源：http://ifh.cqqwz.cn

*)     echo "未知命令" ;;
来源：http://zsd.cashguo.top

esac
来源：http://xid.pycfn.com

[R12] for 遍历文件
来源：http://scw.fktsv.cn

for f in *.txt; do echo "$f"; done
来源：http://yjz.nwbrower.top

[R13] for 计数循环
来源：http://zqw.shuidangran.top

for i in {1..10}; do echo "$i"; done
来源：http://dmy.yanxiufei.cn

[R14] C 风格 for
来源：http://nfc.ybcxt.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://izf.fengsongda.top

[R15] while 逐行读文件
来源：http://yni.birdmap.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bfh.bjfxy.top

[R16] until 等待条件
来源：http://vjs.fanxiaobao.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://djt.fanxiaobao.xyz

[R17] 数组定义与取值
来源：http://lyz.chenzaomai.com

arr=(a b c); echo "${arr[0]}"
来源：http://noq.cdnleiting.top

[R18] 遍历数组
来源：http://efq.fengsongda.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zvq.daxiang520.top

[R19] 数组长度
来源：http://lwq.redwolf501.top

echo "${#arr[@]}"
来源：http://uno.wangshuangyany.cn

[R20] 关联数组（字典）
来源：http://spk.dianchejie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://obm.jqgufenzy.top

[R21] 字符串长度
来源：http://dtu.yongpay.top

echo "${#s}"
来源：http://clb.snrcjt.cn

[R22] 截取子串
来源：http://mhq.chenzaomai.com

echo "${s:0:5}"
来源：http://asf.quarkkingdee.top

[R23] 字符串替换
来源：http://tuf.sjlbkw.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vhq.hnqzz.top

[R24] 大小写转换
来源：http://akw.jinyuanbaomall.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nlr.jyoumei.cn

[R25] 去后缀 / 去前缀
来源：http://gqr.yangfankeji.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://zoi.tanke756.top

[R26] 命令替换
来源：http://qbu.zhaomingkeji.xyz

now=$(date +%F); echo "$now"
来源：http://zwu.hfpthk.cn

[R27] 算术展开
来源：http://wuh.jinqigufen.top

echo $((1 + 2 * 3))
来源：http://vpl.tian-w.cn

[R28] 浮点运算
来源：http://iei.hammf.cn

echo "scale=2; 10/3" | bc
来源：http://ejj.uphjek.com

[R29] 定义函数
来源：http://xjy.jiagoushi.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ram.cheryme.top

[R30] 函数返回状态码
来源：http://pnr.shangyingyoupin.top

f() { return 0; }; f || echo "失败了"
来源：http://bud.feifeiyinyue.top

[R31] 局部变量
来源：http://xnw.sjlbkw.cn

f() { local x=1; echo "$x"; }
来源：http://nak.nanxinkj.top

[R32] 参数个数校验
来源：http://caf.cheryme.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cvc.gogol.net.cn

[R33] 捕获错误并提示行号
来源：http://tfp.316326.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bbh.jiagoushi.top

[R34] 退出时清理
来源：http://hwd.redwolf501.top

trap 'rm -f "$tmp"' EXIT
来源：http://jsv.zhiwuduotai.top

[R35] 后台执行并等待
来源：http://ivf.c1oappe.top

sleep 5 & pid=$!; wait "$pid"
来源：http://oty.vqdsnc.cn

[R36] 并发执行多个任务
来源：http://kfd.xuetiantiany.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://aop.epnwcf.com

[R37] 把输出赋给变量
来源：http://gcg.ydjk.org.cn

files=$(ls -1)
来源：http://jwf.jinghuilouyu.cn

[R38] 管道串联
来源：http://pbe.ydjk.org.cn

cat a.txt | grep -i error | wc -l
来源：http://tae.yongpay.top

[R39] 重定向标准输出与错误
来源：http://ooz.ywan-chungtsiang.top

cmd > out.log 2>&1
来源：http://rkf.hysaishi.cn

[R40] 追加写日志
来源：http://jyj.yangfankeji.com

echo "log" >> out.log
来源：http://mdy.kuanghao11.cn

[R41] 丢弃输出
来源：http://yni.gogol.net.cn

cmd >/dev/null 2>&1
来源：http://idi.birdmap.top

[R42] 输入重定向
来源：http://mtj.ehwqpu.com

wc -l < a.txt
来源：http://smc.52xcode.cn

[R43] 按名字查找文件
来源：http://efs.epnwcf.com

find . -name "*.log" -type f
来源：http://obm.yfazqb.com

[R44] 按修改时间查找
来源：http://wmn.xylfe.cn

find . -mtime -7 -type f
来源：http://mgy.uphjek.com

[R45] 批量删除
来源：http://sfn.mhx1999.top

find . -name "*.tmp" -delete
来源：http://dbc.hongshengwenyu.top

[R46] 递归替换文件内容
来源：http://iwk.52xcode.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ldr.birdmap.top

[R47] sed 单行替换
来源：http://pyj.nanxuanxn.top

sed -i 's/foo/bar/g' a.txt
来源：http://yqp.ydzc1.top

[R48] awk 取指定列
来源：http://bdq.gogol.net.cn

awk '{print $1, $3}' a.txt
来源：http://yrm.daxiang520.top

[R49] awk 带条件
来源：http://oat.fengsongda.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cao.zycfv.cn

[R50] awk 求和
来源：http://glh.sxryk.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qbb.tianlin.xyz

[R51] 排序去重取前几
来源：http://sjb.zhijiandao.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rio.hcnkem.com

[R52] 统计行数
来源：http://jsi.wangdashe.top

wc -l a.txt
来源：http://pwt.birdmap.top

[R53] 查看文件头与实时尾
来源：http://tsi.zhengqikj.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://luh.jianghu66.top

[R54] 比较两个文件
来源：http://ucr.zhixingplan.top

diff a.txt b.txt
来源：http://vfi.kuanghao11.cn

[R55] 压缩与解压
来源：http://zrr.feifeiyinyue.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zal.snrcjt.cn

[R56] 远程拷贝
来源：http://qui.daria6918.cn

scp file user@host:/path/
来源：http://pkc.gaohongyu789.top

[R57] 远程执行命令
来源：http://tms.jqgfzy.top

ssh user@host 'uptime'
来源：http://use.andypj.xyz

[R58] 下载文件
来源：http://gwm.havefunace.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dft.yuxming.cn

[R59] 发 POST JSON
来源：http://pxx.ydjk.org.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ghg.bjfxy.top

[R60] 只看 HTTP 状态码
来源：http://oak.aibaodan.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://huc.ywan-chungtsiang.top

[R61] 磁盘占用
来源：http://eat.ehwqpu.com

df -h;  du -sh *
来源：http://qcj.snrcjt.cn

[R62] 找最占空间的文件
来源：http://jvw.xingfuxueyuan.xyz

du -ah . | sort -rh | head -10
来源：http://okq.bbcook.cn

[R63] 内存与进程
来源：http://ash.tianlin.xyz

free -h;  ps aux | grep nginx
来源：http://jkh.shangyingyoupin.top

[R64] 结束进程
来源：http://uao.kuanghao11.cn

kill -9 $(pgrep -f app.py)
来源：http://hyj.bjfxy.top

[R65] 查看端口占用
来源：http://shl.daria6918.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://esb.daria6918.cn

[R66] 定时任务
来源：http://kck.yfazqb.com

crontab -e;  crontab -l
来源：http://mfm.chenzaomai.com

[R67] 生成随机十六进制串
来源：http://bmo.chenlongwang.top

openssl rand -hex 16
来源：http://srn.yvedp.cn

[R68] 计算文件校验值
来源：http://qzm.jqgufenzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://wvz.316326.xyz

[R69] 生成随机密码
来源：http://vrf.fktsv.cn

head -c 16 /dev/urandom | base64
来源：http://cya.xinyue.icu

[R70] 时间戳与互转
来源：http://iti.guowangkeji.top

date +%s;  date -d @1700000000
来源：http://cnk.gotoacloud.top

[R71] 日期格式化
来源：http://fxw.tarul.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zdx.wangshuangyany.cn

[R72] 等待端口就绪
来源：http://piw.jqgufenzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://elf.aibaodan.cn

[R73] 分割大日志
来源：http://lns.hysaishi.cn

split -l 1000 big.log part_
来源：http://iwk.zhixingplan.top

[R74] 批量重命名
来源：http://atc.hysaishi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gyn.ydjk.org.cn

[R75] 导出环境变量
来源：http://yhj.chenzaomai.com

export PATH="$HOME/bin:$PATH"
来源：http://snx.daxiang520.top

[R76] 使用临时文件
来源：http://iqx.zhixingplan.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://maj.fanxiaobao.xyz

[R77] 读取用户输入
来源：http://jjc.zhiwuduotai.top

read -rp "请输入: " ans
来源：http://mcq.zhaomingkeji.xyz

[R78] 交互式菜单
来源：http://ymi.shuidangran.top

select opt in a b c; do echo "$opt"; break; done
来源：http://oog.tian-w.cn

[R79] 解析命令行选项
来源：http://qqs.sjlbkw.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ejr.smart0.xyz

[R80] 查看脚本执行耗时
来源：http://ofw.fzhhl.top

time ./run.sh
来源：http://cdt.316326.xyz

================================================================================
来源：http://epz.hnqzz.top

S. C / C++ 专题
来源：http://rsk.ydzc1.top

================================================================================
来源：http://rvj.vqdsnc.cn

[S01] C：Hello World
来源：http://anv.kuanghao11.cn

#include <stdio.h>
来源：http://zuf.fktsv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pvf.redwolf501.top

[S02] C：变量与格式化输出
来源：http://mkp.hcnkem.com

int a = 10; printf("%d\n", a);
来源：http://eha.zhiwuduotai.top

[S03] C：读入整数
来源：http://plq.zhijiandao.cn

int x; scanf("%d", &x);
来源：http://bpi.ctjpmb.com

[S04] C：字符串复制
来源：http://kcm.zhixingplan.top

char dst[32]; strcpy(dst, "hi");
来源：http://ttg.svipenyu.cn

[S05] C：字符串长度
来源：http://ojj.tianlin.xyz

strlen(s)
来源：http://jnd.birdmap.top

[S06] C：字符串比较
来源：http://bsz.pycfn.com

strcmp(a, b) == 0
来源：http://qnr.snrcjt.cn

[S07] C：数组遍历求和
来源：http://ute.xuanzx.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ace.jinqigfzy.top

[S08] C：动态内存分配与释放
来源：http://cwl.xingfuxueyuan.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qwq.wangdashe.top

[S09] C：结构体定义与初始化
来源：http://vmf.pycfn.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zwj.tianlin.xyz

[S10] C：指针与解引用
来源：http://fol.gaohongyu789.top

int *p = &a;  *p = 5;
来源：http://gjt.ydjk.org.cn

[S11] C：逐行读文件
来源：http://tvs.wangdashe.top

FILE *f = fopen("a.txt", "r");
来源：http://xpa.ivvv.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://dax.aizwys.cn

fclose(f);
来源：http://wbp.birdmap.top

[S12] C：写文件
来源：http://wln.shuidangran.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sgd.pengpengdd.cyou

[S13] C：宏定义
来源：http://mql.zycfv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nap.yongpay.top

[S14] C：枚举
来源：http://cmn.dianchejie.cn

enum Color { RED, GREEN, BLUE };
来源：http://yjj.vqdsnc.cn

[S15] C：类型转换
来源：http://yxb.ydzc1.top

(double) a / b
来源：http://gck.pycfn.com

[S16] C：位操作置位
来源：http://hqo.zhoulong.xyz

x |= (1 << 3);
来源：http://sbw.sweek.top

[S17] C：安全拼接字符串
来源：http://nyf.jianghu66.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uzy.tianlin.xyz

[S18] C：命令行参数
来源：http://ich.tanke756.top

int main(int argc, char **argv)
来源：http://lvi.yj202588.top

[S19] C：快速排序
来源：http://kvr.fengsongda.top

qsort(a, n, sizeof(int), cmp);
来源：http://zzg.gogol.net.cn

[S20] C：二分查找
来源：http://gjh.haohaochexian.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wmw.jqgufenzy.top

[S21] C：字符类别判断
来源：http://fzl.jinyuanbaomall.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mvr.hammf.cn

[S22] C：字符串转数字
来源：http://ekx.pengpengdd.cyou

atoi("42");  strtod("3.14", NULL);
来源：http://opt.yongpay.top

[S23] C：随机数
来源：http://dmz.cqqwz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://sih.cashguo.top

[S24] C：获取本地时间
来源：http://fgu.chenjidiqi.icu

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sdv.zhongyouzk.top

[S25] C：内存拷贝
来源：http://hnd.pycfn.com

memcpy(dst, src, n);
来源：http://uvh.iojbl.cn

[S26] C：内存清零
来源：http://iuz.chenlongwang.top


<!-- 参考信息 -->