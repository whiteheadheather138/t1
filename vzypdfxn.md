代发 wailian999

[Q76] 按天统计
来源：http://yvv.svipenyu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wat.yuanzhike.top

[Q77] 时间加减
来源：http://ils.sjlbkw.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qqv.zdqjudy.top

[Q78] 当前时间
来源：http://azi.zdqjudy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wvb.guowangkeji.top

[Q79] 字符串拼接
来源：http://qsc.xuetiantiany.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://izw.jinqigufen.top

[Q80] 字符串截取
来源：http://fkx.epnwcf.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hal.yuanzhike.top

[Q81] 字符串替换
来源：http://mwk.xinyue.icu

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vcm.jinqigufen.top

[Q82] 字符长度与字节长度
来源：http://nar.shanyushiyangtech.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lru.c1oappe.top

[Q83] 大小写转换
来源：http://qwa.yuxming.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jap.hesvh.cn

[Q84] 去除首尾空格
来源：http://ahd.ybcxt.top

SELECT TRIM(name) FROM users;
来源：http://wkz.fzhhl.top

[Q85] 数值取整
来源：http://cyw.tian-w.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://acf.xinyue.icu

[Q86] 读取 JSON 字段
来源：http://wtw.snrcjt.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kmv.c1oappe.top

[Q87] JSON 字段做条件
来源：http://pwf.ivvv.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://opt.aibaodan.cn

[Q88] 行转列（条件聚合）
来源：http://mbn.ivvv.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://naa.ydzc1.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yqg.uphjek.com

[Q89] 判断表是否存在
来源：http://qmo.chenlongwang.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rpv.tarul.cn

[Q90] 生成序号列
来源：http://phr.fzhhl.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xzr.dianchejie.cn

================================================================================
来源：http://hfw.zycfv.cn

R. Bash 专题
来源：http://thh.zhaomingkeji.xyz

================================================================================
来源：http://epq.smart0.xyz

[R01] shebang 与严格模式
来源：http://oxp.zhaomingkeji.xyz

#!/usr/bin/env bash
来源：http://xzu.fzhhl.top

set -euo pipefail
来源：http://con.xinyue.icu

[R02] 变量赋值与使用
来源：http://aud.yueranfly.top

name="Tom"; echo "$name"
来源：http://drv.jlsjyb.cn

[R03] 只读变量
来源：http://gfq.shanyushiyangtech.top

readonly PI=3.14
来源：http://wis.jiagoushi.top

[R04] 位置参数
来源：http://ktm.hywenlv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tdd.vqdsnc.cn

[R05] 参数默认值
来源：http://fbt.svipenyu.cn

name="${1:-default}"
来源：http://ctz.ctjpmb.com

[R06] 判断命令是否存在
来源：http://lkb.yfazqb.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://elh.hywenlv.cn

[R07] if 判断文件
来源：http://jnm.yuanzhike.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://asj.9152youxi.cn

[R08] 数值比较
来源：http://tmt.chenzaomai.com

if (( a > b )); then echo "a 更大"; fi
来源：http://uut.hesvh.cn

[R09] 字符串比较
来源：http://lqo.pengpengdd.cyou

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cwh.9152youxi.cn

[R10] 正则匹配
来源：http://gjj.ywan-chungtsiang.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dev.shuidangran.top

[R11] case 多分支
来源：http://ayh.jianghu66.top

case "$1" in
来源：http://fjj.feifeiyinyue.top

start) echo "启动" ;;
来源：http://itq.hysaishi.cn

stop)  echo "停止" ;;
来源：http://wha.zhengqikj.top

*)     echo "未知命令" ;;
来源：http://qpi.daria6918.cn

esac
来源：http://nyz.xuetiantiany.cn

[R12] for 遍历文件
来源：http://uun.shuidangran.top

for f in *.txt; do echo "$f"; done
来源：http://pmd.kuanghao11.cn

[R13] for 计数循环
来源：http://lqu.aizwys.cn

for i in {1..10}; do echo "$i"; done
来源：http://thy.ppjwa.cn

[R14] C 风格 for
来源：http://tof.jqgufenzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qzv.fzhhl.top

[R15] while 逐行读文件
来源：http://uaw.meibo888.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uim.hywenlv.cn

[R16] until 等待条件
来源：http://rgl.zycfv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bkd.ctjpmb.com

[R17] 数组定义与取值
来源：http://rge.xingfuxueyuan.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://pqz.jianghu66.top

[R18] 遍历数组
来源：http://qjv.zhaomingkeji.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://iro.wangshuangyany.cn

[R19] 数组长度
来源：http://oha.xingfuxueyuan.xyz

echo "${#arr[@]}"
来源：http://asj.fehbvm.com

[R20] 关联数组（字典）
来源：http://sev.zhijiandao.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dap.uphjek.com

[R21] 字符串长度
来源：http://scz.fanxiaobao.xyz

echo "${#s}"
来源：http://ect.hfpthk.cn

[R22] 截取子串
来源：http://ucn.fengsongda.top

echo "${s:0:5}"
来源：http://vos.shuidangran.top

[R23] 字符串替换
来源：http://eyo.xuetiantiany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mqh.shuidangran.top

[R24] 大小写转换
来源：http://kdb.sweek.top

echo "${s^^}"; echo "${s,,}"
来源：http://ihs.c1oappe.top

[R25] 去后缀 / 去前缀
来源：http://hnx.jiagoushi.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://kcq.ppjwa.cn

[R26] 命令替换
来源：http://pkd.aizwys.cn

now=$(date +%F); echo "$now"
来源：http://vxf.xylfe.cn

[R27] 算术展开
来源：http://isa.hysaishi.cn

echo $((1 + 2 * 3))
来源：http://ukq.ywan-chungtsiang.top

[R28] 浮点运算
来源：http://snb.jinghuilouyu.cn

echo "scale=2; 10/3" | bc
来源：http://ztm.redwolf501.top

[R29] 定义函数
来源：http://xfj.quarkkingdee.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lrb.cdnleiting.top

[R30] 函数返回状态码
来源：http://ueg.hysaishi.cn

f() { return 0; }; f || echo "失败了"
来源：http://hhf.pengpengdd.cyou

[R31] 局部变量
来源：http://svh.fengsongda.top

f() { local x=1; echo "$x"; }
来源：http://izl.pengpengdd.cyou

[R32] 参数个数校验
来源：http://pxb.xingfuxueyuan.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://npk.sufxvd.cn

[R33] 捕获错误并提示行号
来源：http://vit.ehwqpu.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bsk.wangshuangyany.cn

[R34] 退出时清理
来源：http://hoa.sjlbkw.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uio.ydzc1.top

[R35] 后台执行并等待
来源：http://tmq.fengsongda.top

sleep 5 & pid=$!; wait "$pid"
来源：http://eau.jyoumei.cn

[R36] 并发执行多个任务
来源：http://oxa.quarkkingdee.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ush.pengpengdd.cyou

[R37] 把输出赋给变量
来源：http://vmh.jqgfzy.top

files=$(ls -1)
来源：http://vzp.xuanzx.com

[R38] 管道串联
来源：http://plh.yj20258.top

cat a.txt | grep -i error | wc -l
来源：http://djn.guowangkeji.top

[R39] 重定向标准输出与错误
来源：http://hze.shanyushiyangkeji.top

cmd > out.log 2>&1
来源：http://fsx.zhaomingkeji.xyz

[R40] 追加写日志
来源：http://cbb.ctjpmb.com

echo "log" >> out.log
来源：http://pqs.guannengcc.top

[R41] 丢弃输出
来源：http://nsc.vehdjk.com

cmd >/dev/null 2>&1
来源：http://sdb.yongpay.top

[R42] 输入重定向
来源：http://mda.bjfxy.top

wc -l < a.txt
来源：http://mlo.andypj.xyz

[R43] 按名字查找文件
来源：http://wml.xylfe.cn

find . -name "*.log" -type f
来源：http://bzn.gaohongyu789.top

[R44] 按修改时间查找
来源：http://drx.tianlin.xyz

find . -mtime -7 -type f
来源：http://qxx.sysykeji.top

[R45] 批量删除
来源：http://qdk.fktsv.cn

find . -name "*.tmp" -delete
来源：http://hzt.xziqi.cn

[R46] 递归替换文件内容
来源：http://khq.ywan-chungtsiang.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fyb.yuxming.cn

[R47] sed 单行替换
来源：http://avw.daria6918.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nay.hcnkem.com

[R48] awk 取指定列
来源：http://wzk.feifeiyinyue.top

awk '{print $1, $3}' a.txt
来源：http://dsy.yfazqb.com

[R49] awk 带条件
来源：http://edr.bjfxy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ipx.jiagoushi.top

[R50] awk 求和
来源：http://ahk.jinqigfzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://xch.daria6918.cn

[R51] 排序去重取前几
来源：http://buy.ydzc1.top

sort a.txt | uniq -c | sort -rn | head
来源：http://gne.tianlin.xyz

[R52] 统计行数
来源：http://nmi.yueranfly.top

wc -l a.txt
来源：http://phq.jinghuilouyu.cn

[R53] 查看文件头与实时尾
来源：http://qrj.hfpthk.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rkr.shangyingyoupin.top

[R54] 比较两个文件
来源：http://zdt.shangyingyoupin.top

diff a.txt b.txt
来源：http://ihl.pycfn.com

[R55] 压缩与解压
来源：http://tkp.yuxming.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ets.xylfe.cn

[R56] 远程拷贝
来源：http://qjj.guannengcc.top

scp file user@host:/path/
来源：http://dnn.dianchejie.cn

[R57] 远程执行命令
来源：http://nkg.wangdashe.top

ssh user@host 'uptime'
来源：http://jrc.yanxiufei.cn

[R58] 下载文件
来源：http://wnk.chenjidiqi.icu

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://brn.pycfn.com

[R59] 发 POST JSON
来源：http://rwp.yangfankeji.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bdz.sxryk.cn

[R60] 只看 HTTP 状态码
来源：http://rsi.sweek.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pci.yonumen.top

[R61] 磁盘占用
来源：http://psn.pengpengdd.cyou

df -h;  du -sh *
来源：http://hkp.snrcjt.cn

[R62] 找最占空间的文件
来源：http://kvw.aizwys.cn

du -ah . | sort -rh | head -10
来源：http://bic.yuanzhike.top

[R63] 内存与进程
来源：http://nul.zhongyouzk.top

free -h;  ps aux | grep nginx
来源：http://oak.hammf.cn

[R64] 结束进程
来源：http://cfr.bbcook.cn

kill -9 $(pgrep -f app.py)
来源：http://dho.wangshuangyany.cn

[R65] 查看端口占用
来源：http://otn.kuanghao11.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mtp.yongpay.top

[R66] 定时任务
来源：http://cwl.aibaodan.cn

crontab -e;  crontab -l
来源：http://vwl.haohaochexian.top

[R67] 生成随机十六进制串
来源：http://jma.yuxming.cn

openssl rand -hex 16
来源：http://zrd.wangshuangyany.cn

[R68] 计算文件校验值
来源：http://fqu.ywan-chungtsiang.top

sha256sum a.txt;  md5sum a.txt
来源：http://koj.ywan-chungtsiang.top

[R69] 生成随机密码
来源：http://hyi.guowangkeji.top

head -c 16 /dev/urandom | base64
来源：http://bjy.guowangkeji.top

[R70] 时间戳与互转
来源：http://rjl.hywenlv.cn

date +%s;  date -d @1700000000
来源：http://dab.aizwys.cn

[R71] 日期格式化
来源：http://kzb.yj20258888.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://iuq.meibo888.top

[R72] 等待端口就绪
来源：http://ebi.ehwqpu.com

until nc -z localhost 3306; do sleep 1; done
来源：http://ulr.chenlongwang.top

[R73] 分割大日志
来源：http://nhe.ydzc1.top

split -l 1000 big.log part_
来源：http://ofl.ppjwa.cn

[R74] 批量重命名
来源：http://anj.hnxiangtu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lxo.fanxiaobao.xyz

[R75] 导出环境变量
来源：http://mfo.uphjek.com

export PATH="$HOME/bin:$PATH"
来源：http://eca.daxiang520.top

[R76] 使用临时文件
来源：http://wou.wangdashe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qxi.cqqwz.cn

[R77] 读取用户输入
来源：http://aws.bbcook.cn

read -rp "请输入: " ans
来源：http://kkz.pycfn.com

[R78] 交互式菜单
来源：http://ygd.xuanzx.com

select opt in a b c; do echo "$opt"; break; done
来源：http://jgx.yj202588.top

[R79] 解析命令行选项
来源：http://lgm.xingfuxueyuan.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://inv.ydjk.org.cn

[R80] 查看脚本执行耗时
来源：http://trb.redwolf501.top

time ./run.sh
来源：http://xpt.ywan-chungtsiang.top

================================================================================
来源：http://dsn.ehwqpu.com

S. C / C++ 专题
来源：http://xqz.hysaishi.cn

================================================================================
来源：http://nkc.sweek.top

[S01] C：Hello World
来源：http://pbb.ivvv.top

#include <stdio.h>
来源：http://oye.tarul.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mon.fktsv.cn

[S02] C：变量与格式化输出
来源：http://tgn.gotoacloud.top

int a = 10; printf("%d\n", a);
来源：http://kjk.sjlbkw.cn

[S03] C：读入整数
来源：http://iri.yj20258888.top

int x; scanf("%d", &x);
来源：http://img.fktsv.cn

[S04] C：字符串复制
来源：http://xtz.dashuyun.cn

char dst[32]; strcpy(dst, "hi");
来源：http://irk.havefunace.top

[S05] C：字符串长度
来源：http://ydn.hfpthk.cn

strlen(s)
来源：http://hdn.jinqigfzy.top

[S06] C：字符串比较
来源：http://jye.yvedp.cn

strcmp(a, b) == 0
来源：http://fys.vehdjk.com

[S07] C：数组遍历求和
来源：http://oqa.yfazqb.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vcr.jqgfzy.top

[S08] C：动态内存分配与释放
来源：http://qov.yj20258888.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ble.xziqi.cn

[S09] C：结构体定义与初始化
来源：http://cap.ppjwa.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sug.chenlongwang.top

[S10] C：指针与解引用
来源：http://aqj.bjfxy.top

int *p = &a;  *p = 5;
来源：http://kxa.daxiang520.top

[S11] C：逐行读文件
来源：http://vpf.hammf.cn

FILE *f = fopen("a.txt", "r");
来源：http://zqy.vqdsnc.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://uls.zhixingplan.top

fclose(f);
来源：http://lce.jianghu66.top

[S12] C：写文件
来源：http://oze.shuidangran.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wec.c1oappe.top

[S13] C：宏定义
来源：http://lbw.hcnkem.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fjn.yuanzhike.top

[S14] C：枚举
来源：http://uht.ybcxt.top

enum Color { RED, GREEN, BLUE };
来源：http://znn.shuidangran.top

[S15] C：类型转换
来源：http://irq.fktsv.cn

(double) a / b
来源：http://qhc.cucudq.cn

[S16] C：位操作置位
来源：http://njg.hywenlv.cn

x |= (1 << 3);
来源：http://upj.bjfxy.top

[S17] C：安全拼接字符串
来源：http://tor.kuanghao11.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ydl.chenzaomai.com

[S18] C：命令行参数
来源：http://uvk.dianchejie.cn

int main(int argc, char **argv)
来源：http://kdo.yuanzhike.top

[S19] C：快速排序
来源：http://cek.snrcjt.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dwx.snrcjt.cn

[S20] C：二分查找
来源：http://guc.yuanzhike.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rwb.tanke756.top

[S21] C：字符类别判断
来源：http://zkk.redwolf501.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cgg.xylfe.cn

[S22] C：字符串转数字
来源：http://uae.zhoulong.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://gja.guowangkeji.top

[S23] C：随机数
来源：http://jfq.jyoumei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zjz.hnxiangtu.top

[S24] C：获取本地时间
来源：http://syz.gzhubu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rbz.cashguo.top

[S25] C：内存拷贝
来源：http://zuu.guannengcc.top

memcpy(dst, src, n);
来源：http://ztz.xuetiantiany.cn

[S26] C：内存清零
来源：http://ewo.mhx1999.top

memset(a, 0, sizeof a);
来源：http://anh.wangshuangyany.cn

[S27] C：定义常量
来源：http://stw.ivvv.top

const double PI = 3.14159;
来源：http://fst.zhixingplan.top

[S28] C：静态变量
来源：http://gvd.xuanzx.com

static int counter = 0;
来源：http://noo.aibaodan.cn

[S29] C：变参函数
来源：http://yct.yvedp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uuh.jinghuilouyu.cn

[S30] C：头文件保护
来源：http://kjg.nanxinkj.top

#ifndef X_H
来源：http://qcm.jinqigfzy.top

#define X_H
来源：http://kwl.cashguo.top

#endif
来源：http://psx.shanyushiyangkeji.top

[S31] C++：Hello World
来源：http://sne.jqgufenzy.top

#include <iostream>
来源：http://bob.9152youxi.cn

int main() { std::cout << "Hello\n"; }
来源：http://imv.zhiwuduotai.top

[S32] C++：字符串
来源：http://avy.yj20258.top

std::string s = "hi";  s += "!";
来源：http://ezi.xingfuxueyuan.xyz

[S33] C++：vector 增删
来源：http://sum.xuetiantiany.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zou.zhixingplan.top

[S34] C++：遍历 vector
来源：http://fnu.tian-w.cn

for (auto &x : v) { std::cout << x; }
来源：http://hjf.snrcjt.cn

[S35] C++：map
来源：http://dln.ehwqpu.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rxz.jqgufenzy.top

[S36] C++：unordered_map
来源：http://ofg.nwbrower.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gfb.aibaodan.cn

[S37] C++：set
来源：http://kjh.xingfuxueyuan.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vac.yvedp.cn

[S38] C++：排序
来源：http://oul.zdbjq.cn

std::sort(v.begin(), v.end());
来源：http://pqu.mhx1999.top

[S39] C++：自定义比较器排序
来源：http://emf.nanxuanxn.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zjc.pengpengdd.cyou

[S40] C++：查找元素
来源：http://dee.shuidangran.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hav.yongpay.top

[S41] C++：类与构造函数
来源：http://zdf.hammf.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://anq.jianghu66.top

[S42] C++：继承与虚函数
来源：http://eyf.bjfxy.top

class B : public Base { public: void f() override {} };
来源：http://aty.xylfe.cn

[S43] C++：智能指针
来源：http://hhb.andypj.xyz

auto p = std::make_unique<int>(5);
来源：http://yth.iojbl.cn

[S44] C++：引用传参
来源：http://icq.cashguo.top

void inc(int &x) { ++x; }
来源：http://wwz.wangdashe.top

[S45] C++：lambda
来源：http://rch.yuanzhike.top

auto add = [](int a, int b) { return a + b; };
来源：http://zwa.yvedp.cn

[S46] C++：函数模板
来源：http://krt.aizwys.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lna.fzhhl.top


<!-- 参考信息 -->