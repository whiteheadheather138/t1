代发 wailian999

ROLLBACK TO sp1;
来源：http://ppd.bjfxy.top

[Q69] 查看执行计划
来源：http://njw.xylfe.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://eve.xuanzx.com

[Q70] 更新统计信息
来源：http://fwa.yj20258888.top

ANALYZE TABLE users;
来源：http://fgg.zycfv.cn

[Q71] 查看建表语句
来源：http://hzn.jlsjyb.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bjo.dashuyun.cn

[Q72] 查看索引
来源：http://sga.xinyue.icu

SHOW INDEX FROM users;
来源：http://wsw.tarul.cn

[Q73] 查看表状态
来源：http://rzr.jiagoushi.top

SHOW TABLE STATUS LIKE 'users';
来源：http://lhc.ydjk.org.cn

[Q74] 强制使用索引
来源：http://tts.sysykeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zkx.ybcxt.top

[Q75] 日期格式化
来源：http://esl.nwbrower.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dsj.nanxinkj.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tft.wangshuangyany.cn

[Q76] 按天统计
来源：http://org.kuanghao11.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zkr.gotoacloud.top

[Q77] 时间加减
来源：http://uwq.pycfn.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bfo.yj20258.top

[Q78] 当前时间
来源：http://fiy.sxryk.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bhu.fzhhl.top

[Q79] 字符串拼接
来源：http://nwr.havefunace.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jym.jiagoushi.top

[Q80] 字符串截取
来源：http://fnq.yanxiufei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bsm.cdnleiting.top

[Q81] 字符串替换
来源：http://dys.ybcxt.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tbf.gaohongyu789.top

[Q82] 字符长度与字节长度
来源：http://gqw.shanyushiyangtech.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dth.vqdsnc.cn

[Q83] 大小写转换
来源：http://ies.jinqigfzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dzp.yangfankeji.com

[Q84] 去除首尾空格
来源：http://avm.sweek.top

SELECT TRIM(name) FROM users;
来源：http://fse.aizwys.cn

[Q85] 数值取整
来源：http://gzc.cqqwz.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nqn.chenlongwang.top

[Q86] 读取 JSON 字段
来源：http://fjn.ctjpmb.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tuo.hongshengwenyu.top

[Q87] JSON 字段做条件
来源：http://zov.jiagoushi.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://btt.hammf.cn

[Q88] 行转列（条件聚合）
来源：http://rgx.yuxming.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bpu.zhijiandao.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yxj.0kj1m.cn

[Q89] 判断表是否存在
来源：http://fnd.jianghu66.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wbn.9152youxi.cn

[Q90] 生成序号列
来源：http://ewo.zhiwuduotai.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qih.epnwcf.com

================================================================================
来源：http://dqw.ivvv.top

R. Bash 专题
来源：http://yko.xylfe.cn

================================================================================
来源：http://mxx.52xcode.cn

[R01] shebang 与严格模式
来源：http://rsi.zdqjudy.top

#!/usr/bin/env bash
来源：http://dsd.sjlbkw.cn

set -euo pipefail
来源：http://cxr.yueranfly.top

[R02] 变量赋值与使用
来源：http://rqn.jiagoushi.top

name="Tom"; echo "$name"
来源：http://fpf.bjfxy.top

[R03] 只读变量
来源：http://sag.hammf.cn

readonly PI=3.14
来源：http://pby.hongshengwenyu.top

[R04] 位置参数
来源：http://scg.snrcjt.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://veu.zhongyouzk.top

[R05] 参数默认值
来源：http://aqr.guowangkeji.top

name="${1:-default}"
来源：http://mbb.yueranfly.top

[R06] 判断命令是否存在
来源：http://sdj.zhiwuduotai.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nbo.wangshuangyany.cn

[R07] if 判断文件
来源：http://isa.316326.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kgn.svipenyu.cn

[R08] 数值比较
来源：http://jlm.jyoumei.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xbs.hywenlv.cn

[R09] 字符串比较
来源：http://yhk.yongpay.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qeq.ivvv.top

[R10] 正则匹配
来源：http://mym.aibaodan.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uel.snrcjt.cn

[R11] case 多分支
来源：http://yno.jinqigfzy.top

case "$1" in
来源：http://gxj.hesvh.cn

start) echo "启动" ;;
来源：http://fwb.yuanzhike.top

stop)  echo "停止" ;;
来源：http://xtx.snrcjt.cn

*)     echo "未知命令" ;;
来源：http://fzy.hammf.cn

esac
来源：http://kgl.chenzaomai.com

[R12] for 遍历文件
来源：http://nnx.jinqigufen.top

for f in *.txt; do echo "$f"; done
来源：http://zwf.cucudq.cn

[R13] for 计数循环
来源：http://xnh.xuanzx.com

for i in {1..10}; do echo "$i"; done
来源：http://egh.kuanghao11.cn

[R14] C 风格 for
来源：http://hju.ywan-chungtsiang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gjc.guannengcc.top

[R15] while 逐行读文件
来源：http://ofe.feifeiyinyue.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cmu.fehbvm.com

[R16] until 等待条件
来源：http://ogi.jqgfzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zsq.ybcxt.top

[R17] 数组定义与取值
来源：http://vwu.sysykeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://ory.vqdsnc.cn

[R18] 遍历数组
来源：http://yzs.epnwcf.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vsl.kuanghao11.cn

[R19] 数组长度
来源：http://kqj.snrcjt.cn

echo "${#arr[@]}"
来源：http://dxd.yj20258.top

[R20] 关联数组（字典）
来源：http://mki.ctjpmb.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://aaj.fktsv.cn

[R21] 字符串长度
来源：http://xvg.shangyingyoupin.top

echo "${#s}"
来源：http://slr.guannengcc.top

[R22] 截取子串
来源：http://rfe.xziqi.cn

echo "${s:0:5}"
来源：http://yic.pengpengdd.cyou

[R23] 字符串替换
来源：http://ylo.xuetiantiany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jag.sxryk.cn

[R24] 大小写转换
来源：http://ich.jinqigfzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://bpq.tian-w.cn

[R25] 去后缀 / 去前缀
来源：http://xjp.fktsv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cyf.hammf.cn

[R26] 命令替换
来源：http://njx.dianchejie.cn

now=$(date +%F); echo "$now"
来源：http://gex.andypj.xyz

[R27] 算术展开
来源：http://vrg.zhoulong.xyz

echo $((1 + 2 * 3))
来源：http://qub.ppjwa.cn

[R28] 浮点运算
来源：http://ifl.dianchejie.cn

echo "scale=2; 10/3" | bc
来源：http://hip.xylfe.cn

[R29] 定义函数
来源：http://fud.aibaodan.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zyg.shanyushiyangtech.top

[R30] 函数返回状态码
来源：http://yjp.aibaodan.cn

f() { return 0; }; f || echo "失败了"
来源：http://awb.shangyingyoupin.top

[R31] 局部变量
来源：http://bav.wangshuangyany.cn

f() { local x=1; echo "$x"; }
来源：http://vmx.hysaishi.cn

[R32] 参数个数校验
来源：http://miw.52xcode.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cym.gogol.net.cn

[R33] 捕获错误并提示行号
来源：http://bgf.aizwys.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rcq.shanyushiyangkeji.top

[R34] 退出时清理
来源：http://bco.jinghuilouyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mpq.bbcook.cn

[R35] 后台执行并等待
来源：http://oxb.sufxvd.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nyd.xziqi.cn

[R36] 并发执行多个任务
来源：http://fno.ivvv.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://trm.ywan-chungtsiang.top

[R37] 把输出赋给变量
来源：http://oan.smart0.xyz

files=$(ls -1)
来源：http://uqq.316326.xyz

[R38] 管道串联
来源：http://kdy.dashuyun.cn

cat a.txt | grep -i error | wc -l
来源：http://wez.chenzaomai.com

[R39] 重定向标准输出与错误
来源：http://yvy.xylfe.cn

cmd > out.log 2>&1
来源：http://yqa.vqdsnc.cn

[R40] 追加写日志
来源：http://koj.ybcxt.top

echo "log" >> out.log
来源：http://eqq.nanxuanxn.top

[R41] 丢弃输出
来源：http://akh.dashuyun.cn

cmd >/dev/null 2>&1
来源：http://znw.haohaochexian.top

[R42] 输入重定向
来源：http://qnh.meibo888.top

wc -l < a.txt
来源：http://kqj.jianghu66.top

[R43] 按名字查找文件
来源：http://pqn.nanxuanxn.top

find . -name "*.log" -type f
来源：http://eso.iojbl.cn

[R44] 按修改时间查找
来源：http://ewv.kuanghao11.cn

find . -mtime -7 -type f
来源：http://pqg.zhoulong.xyz

[R45] 批量删除
来源：http://slx.sxryk.cn

find . -name "*.tmp" -delete
来源：http://cee.kuanghao11.cn

[R46] 递归替换文件内容
来源：http://ker.quarkkingdee.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vqd.guannengcc.top

[R47] sed 单行替换
来源：http://zta.shzxlz.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nun.ehwqpu.com

[R48] awk 取指定列
来源：http://pzp.shuidangran.top

awk '{print $1, $3}' a.txt
来源：http://trb.cheryme.top

[R49] awk 带条件
来源：http://arv.yfazqb.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://eek.tianlin.xyz

[R50] awk 求和
来源：http://tft.smart0.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://pwz.xuetiantiany.cn

[R51] 排序去重取前几
来源：http://bnr.ydzc1.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ows.hcnkem.com

[R52] 统计行数
来源：http://zvm.jiagoushi.top

wc -l a.txt
来源：http://ejw.cqqwz.cn

[R53] 查看文件头与实时尾
来源：http://ems.nwbrower.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zcp.c1oappe.top

[R54] 比较两个文件
来源：http://hau.hesvh.cn

diff a.txt b.txt
来源：http://eee.zhixingplan.top

[R55] 压缩与解压
来源：http://ekn.ydzc1.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fic.haohaochexian.top

[R56] 远程拷贝
来源：http://fvx.wangshuangyany.cn

scp file user@host:/path/
来源：http://fok.zhongyouzk.top

[R57] 远程执行命令
来源：http://fyy.yonumen.top

ssh user@host 'uptime'
来源：http://ngz.iojbl.cn

[R58] 下载文件
来源：http://fuk.sweek.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://twe.iojbl.cn

[R59] 发 POST JSON
来源：http://eks.hnqzz.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yba.bjfxy.top

[R60] 只看 HTTP 状态码
来源：http://qhx.fktsv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qaa.hesvh.cn

[R61] 磁盘占用
来源：http://jtx.yfazqb.com

df -h;  du -sh *
来源：http://qmh.chenlongwang.top

[R62] 找最占空间的文件
来源：http://ozv.jlsjyb.cn

du -ah . | sort -rh | head -10
来源：http://sju.sweek.top

[R63] 内存与进程
来源：http://pov.hcnkem.com

free -h;  ps aux | grep nginx
来源：http://eud.fzhhl.top

[R64] 结束进程
来源：http://eed.tarul.cn

kill -9 $(pgrep -f app.py)
来源：http://rqs.daxiang520.top

[R65] 查看端口占用
来源：http://tnb.hammf.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mku.xuetiantiany.cn

[R66] 定时任务
来源：http://cic.daria6918.cn

crontab -e;  crontab -l
来源：http://pfu.yj20258888.top

[R67] 生成随机十六进制串
来源：http://lfk.yj20258.top

openssl rand -hex 16
来源：http://icz.dashuyun.cn

[R68] 计算文件校验值
来源：http://bmg.aibaodan.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mkx.hfpthk.cn

[R69] 生成随机密码
来源：http://amr.hfpthk.cn

head -c 16 /dev/urandom | base64
来源：http://cjs.tanke756.top

[R70] 时间戳与互转
来源：http://nox.shanyushiyangtech.top

date +%s;  date -d @1700000000
来源：http://ftb.hywenlv.cn

[R71] 日期格式化
来源：http://fwj.yueranfly.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://lsw.cdnleiting.top

[R72] 等待端口就绪
来源：http://gwx.hongshengwenyu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://bqe.dianchejie.cn

[R73] 分割大日志
来源：http://lun.fktsv.cn

split -l 1000 big.log part_
来源：http://lfm.ybcxt.top

[R74] 批量重命名
来源：http://txe.tanke756.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rsm.xuanzx.com

[R75] 导出环境变量
来源：http://vqo.zhijiandao.cn

export PATH="$HOME/bin:$PATH"
来源：http://hax.zhaomingkeji.xyz

[R76] 使用临时文件
来源：http://gxv.jinghuilouyu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bpm.sweek.top

[R77] 读取用户输入
来源：http://wsg.ydjk.org.cn

read -rp "请输入: " ans
来源：http://dth.sjlbkw.cn

[R78] 交互式菜单
来源：http://xrb.zhaomingkeji.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://dot.pengpengdd.cyou

[R79] 解析命令行选项
来源：http://ztb.iojbl.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nml.xylfe.cn

[R80] 查看脚本执行耗时
来源：http://rdw.gzhubu.top

time ./run.sh
来源：http://iid.dashuyun.cn

================================================================================
来源：http://vlh.nanxuanxn.top

S. C / C++ 专题
来源：http://iek.gaohongyu789.top

================================================================================
来源：http://fyk.hcnkem.com

[S01] C：Hello World
来源：http://riv.svipenyu.cn

#include <stdio.h>
来源：http://dlo.jianghu66.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://fza.zdbjq.cn

[S02] C：变量与格式化输出
来源：http://yfd.gogol.net.cn

int a = 10; printf("%d\n", a);
来源：http://ovu.nanxuanxn.top

[S03] C：读入整数
来源：http://och.zhengqikj.top

int x; scanf("%d", &x);
来源：http://oih.wangdashe.top

[S04] C：字符串复制
来源：http://jmz.sysykeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://vph.kuanghao11.cn

[S05] C：字符串长度
来源：http://rmn.hfpthk.cn

strlen(s)
来源：http://zrn.ywan-chungtsiang.top

[S06] C：字符串比较
来源：http://zbw.c1oappe.top

strcmp(a, b) == 0
来源：http://dno.svipenyu.cn

[S07] C：数组遍历求和
来源：http://fyo.jyoumei.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cxl.quarkkingdee.top

[S08] C：动态内存分配与释放
来源：http://ydn.zhixingplan.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pvj.yangfankeji.com

[S09] C：结构体定义与初始化
来源：http://bvr.fehbvm.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cbf.pengpengdd.cyou

[S10] C：指针与解引用
来源：http://osh.zhaomingkeji.xyz

int *p = &a;  *p = 5;
来源：http://fry.nwbrower.top

[S11] C：逐行读文件
来源：http://ggo.hywenlv.cn

FILE *f = fopen("a.txt", "r");
来源：http://pvc.hcnkem.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://kgn.chenjidiqi.icu

fclose(f);
来源：http://zcs.hysaishi.cn

[S12] C：写文件
来源：http://nbw.fzhhl.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vqh.cashguo.top

[S13] C：宏定义
来源：http://uko.iojbl.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ekb.wangshuangyany.cn

[S14] C：枚举
来源：http://pae.aibaodan.cn

enum Color { RED, GREEN, BLUE };
来源：http://vol.jianghu66.top

[S15] C：类型转换
来源：http://xxx.epnwcf.com

(double) a / b
来源：http://cdd.haohaochexian.top

[S16] C：位操作置位
来源：http://moz.jinghuilouyu.cn

x |= (1 << 3);
来源：http://iqt.chenlongwang.top

[S17] C：安全拼接字符串
来源：http://rdj.aizwys.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://aif.zhengqikj.top

[S18] C：命令行参数
来源：http://czq.shzxlz.cn

int main(int argc, char **argv)
来源：http://hnq.hnxiangtu.top

[S19] C：快速排序
来源：http://fuy.sysykeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://tpc.sysykeji.top

[S20] C：二分查找
来源：http://kam.birdmap.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eyk.jyoumei.cn

[S21] C：字符类别判断
来源：http://jxl.aizwys.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xpb.hammf.cn

[S22] C：字符串转数字
来源：http://pib.xuetiantiany.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yxa.zhaomingkeji.xyz

[S23] C：随机数
来源：http://ozy.yueranfly.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fro.tian-w.cn

[S24] C：获取本地时间
来源：http://min.yueranfly.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tri.yfazqb.com

[S25] C：内存拷贝
来源：http://sid.jqgfzy.top

memcpy(dst, src, n);
来源：http://rom.andypj.xyz

[S26] C：内存清零
来源：http://bkn.fanxiaobao.xyz

memset(a, 0, sizeof a);
来源：http://dlw.hysaishi.cn

[S27] C：定义常量
来源：http://dop.zhongyouzk.top

const double PI = 3.14159;
来源：http://htq.aizwys.cn

[S28] C：静态变量
来源：http://cxd.uphjek.com

static int counter = 0;
来源：http://idi.fengsongda.top

[S29] C：变参函数
来源：http://quo.xuetiantiany.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xpc.sweek.top

[S30] C：头文件保护
来源：http://nxm.haohaochexian.top

#ifndef X_H
来源：http://ism.jinqigfzy.top

#define X_H
来源：http://ngp.vqdsnc.cn

#endif
来源：http://ipp.yj20258.top

[S31] C++：Hello World
来源：http://izt.shangyingyoupin.top

#include <iostream>
来源：http://dos.xingfuxueyuan.xyz

int main() { std::cout << "Hello\n"; }
来源：http://vjd.yongpay.top

[S32] C++：字符串
来源：http://vzt.xinyue.icu

std::string s = "hi";  s += "!";
来源：http://vrz.jlsjyb.cn

[S33] C++：vector 增删
来源：http://cjl.vqdsnc.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pjd.hesvh.cn

[S34] C++：遍历 vector
来源：http://smo.jianghu66.top

for (auto &x : v) { std::cout << x; }
来源：http://eyr.jinqigufen.top

[S35] C++：map
来源：http://fap.ydjk.org.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://stj.hesvh.cn

[S36] C++：unordered_map
来源：http://pfk.quarkkingdee.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://liy.ehwqpu.com

[S37] C++：set
来源：http://gxv.c1oappe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rmr.shzxlz.cn

[S38] C++：排序
来源：http://vdv.zhixingplan.top

std::sort(v.begin(), v.end());
来源：http://fzg.havefunace.top


<!-- 参考信息 -->