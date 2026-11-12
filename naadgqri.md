代发 wailian999

ANALYZE TABLE users;
来源：http://zkk.yuanzhike.top

[Q71] 查看建表语句
来源：http://gsv.bjfxy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pbx.hesvh.cn

[Q72] 查看索引
来源：http://jtz.sjlbkw.cn

SHOW INDEX FROM users;
来源：http://iil.yj20258.top

[Q73] 查看表状态
来源：http://mfq.zycfv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://voq.wangshuangyany.cn

[Q74] 强制使用索引
来源：http://jxo.zycfv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tbw.tianlin.xyz

[Q75] 日期格式化
来源：http://ich.shanyushiyangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jka.shanyushiyangtech.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jov.haohaochexian.top

[Q76] 按天统计
来源：http://kfn.shanyushiyangkeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ccj.nanxuanxn.top

[Q77] 时间加减
来源：http://aim.jyoumei.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fvq.zhijiandao.cn

[Q78] 当前时间
来源：http://hmx.nwbrower.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bmd.gzhubu.top

[Q79] 字符串拼接
来源：http://qvr.xylfe.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hif.zycfv.cn

[Q80] 字符串截取
来源：http://pxv.hfpthk.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://peq.iojbl.cn

[Q81] 字符串替换
来源：http://ixs.epnwcf.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rea.redwolf501.top

[Q82] 字符长度与字节长度
来源：http://jld.hysaishi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zeg.nanxuanxn.top

[Q83] 大小写转换
来源：http://tui.aizwys.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yiu.jyoumei.cn

[Q84] 去除首尾空格
来源：http://qdg.zhongyouzk.top

SELECT TRIM(name) FROM users;
来源：http://wsk.fktsv.cn

[Q85] 数值取整
来源：http://vwg.bjfxy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tdx.ywan-chungtsiang.top

[Q86] 读取 JSON 字段
来源：http://mwh.kuanghao11.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pjo.sysykeji.top

[Q87] JSON 字段做条件
来源：http://pxk.zhaomingkeji.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gef.epnwcf.com

[Q88] 行转列（条件聚合）
来源：http://hrf.jqgfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hxl.hywenlv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cnu.jianghu66.top

[Q89] 判断表是否存在
来源：http://lwq.hnxiangtu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vgz.yvedp.cn

[Q90] 生成序号列
来源：http://pyy.dianchejie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kfu.shuidangran.top

================================================================================
来源：http://ooo.haohaochexian.top

R. Bash 专题
来源：http://khv.yuxming.cn

================================================================================
来源：http://bgf.vqdsnc.cn

[R01] shebang 与严格模式
来源：http://wln.guowangkeji.top

#!/usr/bin/env bash
来源：http://lqb.dianchejie.cn

set -euo pipefail
来源：http://xmk.hesvh.cn

[R02] 变量赋值与使用
来源：http://tht.zycfv.cn

name="Tom"; echo "$name"
来源：http://nqs.jlsjyb.cn

[R03] 只读变量
来源：http://wvy.sufxvd.cn

readonly PI=3.14
来源：http://zos.ivvv.top

[R04] 位置参数
来源：http://tya.shzxlz.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mds.kuanghao11.cn

[R05] 参数默认值
来源：http://ipn.zhaomingkeji.xyz

name="${1:-default}"
来源：http://eyu.wangdashe.top

[R06] 判断命令是否存在
来源：http://bbi.daria6918.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mon.jyoumei.cn

[R07] if 判断文件
来源：http://ocn.hcnkem.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xpn.svipenyu.cn

[R08] 数值比较
来源：http://wen.nanxuanxn.top

if (( a > b )); then echo "a 更大"; fi
来源：http://epw.zhaomingkeji.xyz

[R09] 字符串比较
来源：http://aje.hfpthk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wyt.0kj1m.cn

[R10] 正则匹配
来源：http://svf.shuidangran.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pfo.xuanzx.com

[R11] case 多分支
来源：http://xlm.shuidangran.top

case "$1" in
来源：http://cjj.zhoulong.xyz

start) echo "启动" ;;
来源：http://vyf.sysykeji.top

stop)  echo "停止" ;;
来源：http://zry.meibo888.top

*)     echo "未知命令" ;;
来源：http://cmh.zhongyouzk.top

esac
来源：http://ctl.jqgufenzy.top

[R12] for 遍历文件
来源：http://vkg.kuanghao11.cn

for f in *.txt; do echo "$f"; done
来源：http://pwb.mhx1999.top

[R13] for 计数循环
来源：http://wew.vqdsnc.cn

for i in {1..10}; do echo "$i"; done
来源：http://bai.yfazqb.com

[R14] C 风格 for
来源：http://jzm.xingfuxueyuan.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ljw.redwolf501.top

[R15] while 逐行读文件
来源：http://fru.fengsongda.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fhp.tianlin.xyz

[R16] until 等待条件
来源：http://wnc.yvedp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://muf.guannengcc.top

[R17] 数组定义与取值
来源：http://zqq.yj20258.top

arr=(a b c); echo "${arr[0]}"
来源：http://gqs.meibo888.top

[R18] 遍历数组
来源：http://vvx.epnwcf.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ine.svipenyu.cn

[R19] 数组长度
来源：http://res.ppjwa.cn

echo "${#arr[@]}"
来源：http://xpz.pycfn.com

[R20] 关联数组（字典）
来源：http://jjd.jqgufenzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hbs.haohaochexian.top

[R21] 字符串长度
来源：http://zss.xuetiantiany.cn

echo "${#s}"
来源：http://umt.xinyue.icu

[R22] 截取子串
来源：http://mkx.ivvv.top

echo "${s:0:5}"
来源：http://sxn.zhongyouzk.top

[R23] 字符串替换
来源：http://sma.bjfxy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jkx.shanyushiyangkeji.top

[R24] 大小写转换
来源：http://ktj.hfpthk.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uke.svipenyu.cn

[R25] 去后缀 / 去前缀
来源：http://kbc.ivvv.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ivb.fzhhl.top

[R26] 命令替换
来源：http://myq.shzxlz.cn

now=$(date +%F); echo "$now"
来源：http://guo.gaohongyu789.top

[R27] 算术展开
来源：http://rhm.uphjek.com

echo $((1 + 2 * 3))
来源：http://pij.snrcjt.cn

[R28] 浮点运算
来源：http://dgq.snrcjt.cn

echo "scale=2; 10/3" | bc
来源：http://aqy.shanyushiyangkeji.top

[R29] 定义函数
来源：http://fxy.xuanzx.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://eys.316326.xyz

[R30] 函数返回状态码
来源：http://zrt.jqgufenzy.top

f() { return 0; }; f || echo "失败了"
来源：http://cez.xuetiantiany.cn

[R31] 局部变量
来源：http://ctp.tanke756.top

f() { local x=1; echo "$x"; }
来源：http://jhw.sjlbkw.cn

[R32] 参数个数校验
来源：http://aaj.guannengcc.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zrc.zhongyouzk.top

[R33] 捕获错误并提示行号
来源：http://lgx.shanyushiyangtech.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nib.meibo888.top

[R34] 退出时清理
来源：http://olw.fktsv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lhc.hywenlv.cn

[R35] 后台执行并等待
来源：http://cza.jiagoushi.top

sleep 5 & pid=$!; wait "$pid"
来源：http://olh.cashguo.top

[R36] 并发执行多个任务
来源：http://bel.dianchejie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kii.yanxiufei.cn

[R37] 把输出赋给变量
来源：http://duu.yangfankeji.com

files=$(ls -1)
来源：http://ukl.sweek.top

[R38] 管道串联
来源：http://jpf.jianghu66.top

cat a.txt | grep -i error | wc -l
来源：http://yla.ctjpmb.com

[R39] 重定向标准输出与错误
来源：http://uzm.yuxming.cn

cmd > out.log 2>&1
来源：http://qes.sysykeji.top

[R40] 追加写日志
来源：http://jxq.tian-w.cn

echo "log" >> out.log
来源：http://qoh.hysaishi.cn

[R41] 丢弃输出
来源：http://xrj.birdmap.top

cmd >/dev/null 2>&1
来源：http://pdr.feifeiyinyue.top

[R42] 输入重定向
来源：http://hgw.nanxuanxn.top

wc -l < a.txt
来源：http://ytn.bbcook.cn

[R43] 按名字查找文件
来源：http://lao.tanke756.top

find . -name "*.log" -type f
来源：http://wth.cashguo.top

[R44] 按修改时间查找
来源：http://tmb.jinyuanbaomall.cn

find . -mtime -7 -type f
来源：http://mfy.gotoacloud.top

[R45] 批量删除
来源：http://nbc.feifeiyinyue.top

find . -name "*.tmp" -delete
来源：http://ooo.hnxiangtu.top

[R46] 递归替换文件内容
来源：http://ali.daria6918.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xvi.316326.xyz

[R47] sed 单行替换
来源：http://gxx.daria6918.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jlc.shanyushiyangkeji.top

[R48] awk 取指定列
来源：http://owv.tarul.cn

awk '{print $1, $3}' a.txt
来源：http://mcd.hnxiangtu.top

[R49] awk 带条件
来源：http://dxr.nwbrower.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rkd.hnqzz.top

[R50] awk 求和
来源：http://wug.chenzaomai.com

awk '{s += $2} END {print s}' a.txt
来源：http://dbn.hfpthk.cn

[R51] 排序去重取前几
来源：http://frs.feifeiyinyue.top

sort a.txt | uniq -c | sort -rn | head
来源：http://qaz.tarul.cn

[R52] 统计行数
来源：http://jmy.jiagoushi.top

wc -l a.txt
来源：http://ohv.zhaomingkeji.xyz

[R53] 查看文件头与实时尾
来源：http://lmm.ywan-chungtsiang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hvc.smart0.xyz

[R54] 比较两个文件
来源：http://vog.chenjidiqi.icu

diff a.txt b.txt
来源：http://pbm.ppjwa.cn

[R55] 压缩与解压
来源：http://ivr.wangdashe.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kkr.hfpthk.cn

[R56] 远程拷贝
来源：http://ybq.cqqwz.cn

scp file user@host:/path/
来源：http://zqf.jqgufenzy.top

[R57] 远程执行命令
来源：http://vij.jyoumei.cn

ssh user@host 'uptime'
来源：http://iny.nwbrower.top

[R58] 下载文件
来源：http://esk.jqgfzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://swk.chenzaomai.com

[R59] 发 POST JSON
来源：http://iga.fzhhl.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bvr.cheryme.top

[R60] 只看 HTTP 状态码
来源：http://nca.jqgufenzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rfa.sweek.top

[R61] 磁盘占用
来源：http://gdw.sysykeji.top

df -h;  du -sh *
来源：http://roq.birdmap.top

[R62] 找最占空间的文件
来源：http://isy.aibaodan.cn

du -ah . | sort -rh | head -10
来源：http://yml.xinyue.icu

[R63] 内存与进程
来源：http://mne.hnqzz.top

free -h;  ps aux | grep nginx
来源：http://mlx.hysaishi.cn

[R64] 结束进程
来源：http://sty.xingfuxueyuan.xyz

kill -9 $(pgrep -f app.py)
来源：http://kic.aizwys.cn

[R65] 查看端口占用
来源：http://alj.zdqjudy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pll.vqdsnc.cn

[R66] 定时任务
来源：http://foc.cheryme.top

crontab -e;  crontab -l
来源：http://wqj.cdnleiting.top

[R67] 生成随机十六进制串
来源：http://rmd.yonumen.top

openssl rand -hex 16
来源：http://gjn.shuidangran.top

[R68] 计算文件校验值
来源：http://bdx.jqgfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://tqa.cdnleiting.top

[R69] 生成随机密码
来源：http://hci.zdbjq.cn

head -c 16 /dev/urandom | base64
来源：http://nbb.9152youxi.cn

[R70] 时间戳与互转
来源：http://kjh.yongpay.top

date +%s;  date -d @1700000000
来源：http://xbr.tarul.cn

[R71] 日期格式化
来源：http://vpu.guannengcc.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vzg.chenlongwang.top

[R72] 等待端口就绪
来源：http://apw.hywenlv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mgr.fktsv.cn

[R73] 分割大日志
来源：http://hvb.zhixingplan.top

split -l 1000 big.log part_
来源：http://iqm.hysaishi.cn

[R74] 批量重命名
来源：http://slo.jinyuanbaomall.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qmm.dashuyun.cn

[R75] 导出环境变量
来源：http://sib.shzxlz.cn

export PATH="$HOME/bin:$PATH"
来源：http://sij.chenlongwang.top

[R76] 使用临时文件
来源：http://aux.gaohongyu789.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mna.52xcode.cn

[R77] 读取用户输入
来源：http://uxv.yueranfly.top

read -rp "请输入: " ans
来源：http://hlc.sjlbkw.cn

[R78] 交互式菜单
来源：http://msz.andypj.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://bug.yonumen.top

[R79] 解析命令行选项
来源：http://qqd.svipenyu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jed.yueranfly.top

[R80] 查看脚本执行耗时
来源：http://yrj.shzxlz.cn

time ./run.sh
来源：http://gwo.ywan-chungtsiang.top

================================================================================
来源：http://cje.zhongyouzk.top

S. C / C++ 专题
来源：http://xgs.zycfv.cn

================================================================================
来源：http://huq.yj20258888.top

[S01] C：Hello World
来源：http://lsk.redwolf501.top

#include <stdio.h>
来源：http://aah.hammf.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://uun.haohaochexian.top

[S02] C：变量与格式化输出
来源：http://xkr.ppjwa.cn

int a = 10; printf("%d\n", a);
来源：http://swv.xuetiantiany.cn

[S03] C：读入整数
来源：http://fce.wangdashe.top

int x; scanf("%d", &x);
来源：http://ckp.birdmap.top

[S04] C：字符串复制
来源：http://ick.vehdjk.com

char dst[32]; strcpy(dst, "hi");
来源：http://ato.gaohongyu789.top

[S05] C：字符串长度
来源：http://zwr.316326.xyz

strlen(s)
来源：http://lkm.nanxinkj.top

[S06] C：字符串比较
来源：http://xii.gzhubu.top

strcmp(a, b) == 0
来源：http://yza.sjlbkw.cn

[S07] C：数组遍历求和
来源：http://yik.shuidangran.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://poh.shangyingyoupin.top

[S08] C：动态内存分配与释放
来源：http://zwp.jlsjyb.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nyp.chenlongwang.top

[S09] C：结构体定义与初始化
来源：http://zct.shzxlz.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fvw.jinyuanbaomall.cn

[S10] C：指针与解引用
来源：http://wam.xuanzx.com

int *p = &a;  *p = 5;
来源：http://yrv.hnqzz.top

[S11] C：逐行读文件
来源：http://lbs.yueranfly.top

FILE *f = fopen("a.txt", "r");
来源：http://iqf.wangshuangyany.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wag.tarul.cn

fclose(f);
来源：http://fia.yfazqb.com

[S12] C：写文件
来源：http://upq.zhengqikj.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hxb.yonumen.top

[S13] C：宏定义
来源：http://rbr.pycfn.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sbn.uphjek.com

[S14] C：枚举
来源：http://fqt.wangdashe.top

enum Color { RED, GREEN, BLUE };
来源：http://kor.hammf.cn

[S15] C：类型转换
来源：http://qkf.ctjpmb.com

(double) a / b
来源：http://fif.hammf.cn

[S16] C：位操作置位
来源：http://pra.sjlbkw.cn

x |= (1 << 3);
来源：http://kkm.fanxiaobao.xyz

[S17] C：安全拼接字符串
来源：http://qfq.xuanzx.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tet.zdqjudy.top

[S18] C：命令行参数
来源：http://oqq.fengsongda.top

int main(int argc, char **argv)
来源：http://omj.uphjek.com

[S19] C：快速排序
来源：http://odl.xingfuxueyuan.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://uot.0kj1m.cn

[S20] C：二分查找
来源：http://ijm.meibo888.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dkv.aibaodan.cn

[S21] C：字符类别判断
来源：http://eyt.chenlongwang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fso.ppjwa.cn

[S22] C：字符串转数字
来源：http://jgk.yueranfly.top

atoi("42");  strtod("3.14", NULL);
来源：http://ulj.vehdjk.com

[S23] C：随机数
来源：http://yjc.316326.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://tke.epnwcf.com

[S24] C：获取本地时间
来源：http://nct.mhx1999.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dve.jinqigfzy.top

[S25] C：内存拷贝
来源：http://hbq.daxiang520.top

memcpy(dst, src, n);
来源：http://pbj.sysykeji.top

[S26] C：内存清零
来源：http://cbu.jlsjyb.cn

memset(a, 0, sizeof a);
来源：http://oqt.sysykeji.top

[S27] C：定义常量
来源：http://ers.nwbrower.top

const double PI = 3.14159;
来源：http://ecf.yfazqb.com

[S28] C：静态变量
来源：http://dwa.zhiwuduotai.top

static int counter = 0;
来源：http://bmf.hnqzz.top

[S29] C：变参函数
来源：http://vzw.jinqigufen.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vwx.jyoumei.cn

[S30] C：头文件保护
来源：http://jbv.smart0.xyz

#ifndef X_H
来源：http://ihx.sxryk.cn

#define X_H
来源：http://taf.quarkkingdee.top

#endif
来源：http://glz.guannengcc.top

[S31] C++：Hello World
来源：http://ezm.yj202588.top

#include <iostream>
来源：http://ohp.xylfe.cn

int main() { std::cout << "Hello\n"; }
来源：http://pzr.zhengqikj.top

[S32] C++：字符串
来源：http://ntz.yanxiufei.cn

std::string s = "hi";  s += "!";
来源：http://rmh.zhijiandao.cn

[S33] C++：vector 增删
来源：http://wep.zhiwuduotai.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wwx.c1oappe.top

[S34] C++：遍历 vector
来源：http://fvs.9152youxi.cn

for (auto &x : v) { std::cout << x; }
来源：http://jae.zhiwuduotai.top

[S35] C++：map
来源：http://ssw.fktsv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://duv.xylfe.cn

[S36] C++：unordered_map
来源：http://fif.zycfv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bme.cqqwz.cn

[S37] C++：set
来源：http://nfo.gaohongyu789.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pak.tarul.cn

[S38] C++：排序
来源：http://mbr.316326.xyz

std::sort(v.begin(), v.end());
来源：http://jnv.xziqi.cn

[S39] C++：自定义比较器排序
来源：http://yqp.yvedp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bvf.316326.xyz

[S40] C++：查找元素
来源：http://znf.jiagoushi.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fcr.gzhubu.top


<!-- 参考信息 -->