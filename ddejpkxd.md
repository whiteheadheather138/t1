代发 wailian999

[Q76] 按天统计
来源：http://ikc.shzxlz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dwd.nwbrower.top

[Q77] 时间加减
来源：http://okn.smart0.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eei.nanxinkj.top

[Q78] 当前时间
来源：http://ygy.zdqjudy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ark.zhixingplan.top

[Q79] 字符串拼接
来源：http://dhm.xuanzx.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dav.tarul.cn

[Q80] 字符串截取
来源：http://qcm.jyoumei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://eti.chenzaomai.com

[Q81] 字符串替换
来源：http://yye.jiagoushi.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://osn.kuanghao11.cn

[Q82] 字符长度与字节长度
来源：http://uri.kuanghao11.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ljy.316326.xyz

[Q83] 大小写转换
来源：http://pjg.andypj.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tnf.guowangkeji.top

[Q84] 去除首尾空格
来源：http://bpi.fanxiaobao.xyz

SELECT TRIM(name) FROM users;
来源：http://hap.hongshengwenyu.top

[Q85] 数值取整
来源：http://uqq.gotoacloud.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jqu.bbcook.cn

[Q86] 读取 JSON 字段
来源：http://xtf.shanyushiyangtech.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ahs.zhiwuduotai.top

[Q87] JSON 字段做条件
来源：http://pny.feifeiyinyue.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yyq.guowangkeji.top

[Q88] 行转列（条件聚合）
来源：http://dwg.yanxiufei.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qkn.fengsongda.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://srk.vqdsnc.cn

[Q89] 判断表是否存在
来源：http://ylv.xuanzx.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bej.fengsongda.top

[Q90] 生成序号列
来源：http://gtj.shanyushiyangkeji.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rvg.jinghuilouyu.cn

================================================================================
来源：http://gmf.tianlin.xyz

R. Bash 专题
来源：http://juc.quarkkingdee.top

================================================================================
来源：http://suo.meibo888.top

[R01] shebang 与严格模式
来源：http://pln.fktsv.cn

#!/usr/bin/env bash
来源：http://bil.hongshengwenyu.top

set -euo pipefail
来源：http://uwj.xylfe.cn

[R02] 变量赋值与使用
来源：http://hmt.tian-w.cn

name="Tom"; echo "$name"
来源：http://vvb.ybcxt.top

[R03] 只读变量
来源：http://pjl.sxryk.cn

readonly PI=3.14
来源：http://fdk.hesvh.cn

[R04] 位置参数
来源：http://nwy.vehdjk.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://exe.fzhhl.top

[R05] 参数默认值
来源：http://ycv.sysykeji.top

name="${1:-default}"
来源：http://qva.tarul.cn

[R06] 判断命令是否存在
来源：http://ptp.xingfuxueyuan.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zmr.andypj.xyz

[R07] if 判断文件
来源：http://bti.mhx1999.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kfr.chenlongwang.top

[R08] 数值比较
来源：http://iwb.sufxvd.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wkv.vqdsnc.cn

[R09] 字符串比较
来源：http://uzw.meibo888.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hjc.ppjwa.cn

[R10] 正则匹配
来源：http://rxy.haohaochexian.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dyq.xuetiantiany.cn

[R11] case 多分支
来源：http://bwi.tian-w.cn

case "$1" in
来源：http://gpj.sufxvd.cn

start) echo "启动" ;;
来源：http://gmb.nwbrower.top

stop)  echo "停止" ;;
来源：http://qkq.hnxiangtu.top

*)     echo "未知命令" ;;
来源：http://hwl.ppjwa.cn

esac
来源：http://kxp.tanke756.top

[R12] for 遍历文件
来源：http://ztg.tarul.cn

for f in *.txt; do echo "$f"; done
来源：http://wqu.sxryk.cn

[R13] for 计数循环
来源：http://wka.shuidangran.top

for i in {1..10}; do echo "$i"; done
来源：http://ecj.jianghu66.top

[R14] C 风格 for
来源：http://bco.haohaochexian.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iui.jlsjyb.cn

[R15] while 逐行读文件
来源：http://dxf.fengsongda.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cpm.xuetiantiany.cn

[R16] until 等待条件
来源：http://geb.sufxvd.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://eky.ehwqpu.com

[R17] 数组定义与取值
来源：http://nld.smart0.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://hbi.tanke756.top

[R18] 遍历数组
来源：http://tcy.fktsv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xlf.yueranfly.top

[R19] 数组长度
来源：http://ezt.hfpthk.cn

echo "${#arr[@]}"
来源：http://jbj.uphjek.com

[R20] 关联数组（字典）
来源：http://xih.zhaomingkeji.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qgy.hnqzz.top

[R21] 字符串长度
来源：http://ymw.zycfv.cn

echo "${#s}"
来源：http://tyl.havefunace.top

[R22] 截取子串
来源：http://dex.yangfankeji.com

echo "${s:0:5}"
来源：http://att.smart0.xyz

[R23] 字符串替换
来源：http://kbf.ppjwa.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://igg.fzhhl.top

[R24] 大小写转换
来源：http://bby.bbcook.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jzp.fanxiaobao.xyz

[R25] 去后缀 / 去前缀
来源：http://zth.cqqwz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sbe.cqqwz.cn

[R26] 命令替换
来源：http://bom.tarul.cn

now=$(date +%F); echo "$now"
来源：http://cfz.0kj1m.cn

[R27] 算术展开
来源：http://olt.sjlbkw.cn

echo $((1 + 2 * 3))
来源：http://nct.vqdsnc.cn

[R28] 浮点运算
来源：http://vve.hywenlv.cn

echo "scale=2; 10/3" | bc
来源：http://qrh.shangyingyoupin.top

[R29] 定义函数
来源：http://dam.yanxiufei.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rrh.havefunace.top

[R30] 函数返回状态码
来源：http://gbd.kuanghao11.cn

f() { return 0; }; f || echo "失败了"
来源：http://yyx.jiagoushi.top

[R31] 局部变量
来源：http://wis.zhongyouzk.top

f() { local x=1; echo "$x"; }
来源：http://sld.fanxiaobao.xyz

[R32] 参数个数校验
来源：http://zdm.c1oappe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jwa.epnwcf.com

[R33] 捕获错误并提示行号
来源：http://ibs.shanyushiyangtech.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nbw.ybcxt.top

[R34] 退出时清理
来源：http://sjh.ybcxt.top

trap 'rm -f "$tmp"' EXIT
来源：http://zyf.sjlbkw.cn

[R35] 后台执行并等待
来源：http://mna.yanxiufei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kjn.guowangkeji.top

[R36] 并发执行多个任务
来源：http://zbl.guowangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kci.snrcjt.cn

[R37] 把输出赋给变量
来源：http://xdd.hnxiangtu.top

files=$(ls -1)
来源：http://mzv.jinghuilouyu.cn

[R38] 管道串联
来源：http://kft.wangshuangyany.cn

cat a.txt | grep -i error | wc -l
来源：http://vzx.bjfxy.top

[R39] 重定向标准输出与错误
来源：http://osv.yanxiufei.cn

cmd > out.log 2>&1
来源：http://rjy.shanyushiyangtech.top

[R40] 追加写日志
来源：http://avn.chenzaomai.com

echo "log" >> out.log
来源：http://fhz.zhengqikj.top

[R41] 丢弃输出
来源：http://fjj.yuxming.cn

cmd >/dev/null 2>&1
来源：http://vrw.sjlbkw.cn

[R42] 输入重定向
来源：http://mcc.mhx1999.top

wc -l < a.txt
来源：http://tsw.nwbrower.top

[R43] 按名字查找文件
来源：http://uiv.yangfankeji.com

find . -name "*.log" -type f
来源：http://xqg.smart0.xyz

[R44] 按修改时间查找
来源：http://iah.shzxlz.cn

find . -mtime -7 -type f
来源：http://gvu.gaohongyu789.top

[R45] 批量删除
来源：http://fcp.yfazqb.com

find . -name "*.tmp" -delete
来源：http://kwn.shangyingyoupin.top

[R46] 递归替换文件内容
来源：http://wex.xingfuxueyuan.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mjr.yanxiufei.cn

[R47] sed 单行替换
来源：http://zig.cashguo.top

sed -i 's/foo/bar/g' a.txt
来源：http://mhw.hnxiangtu.top

[R48] awk 取指定列
来源：http://jlj.nanxinkj.top

awk '{print $1, $3}' a.txt
来源：http://gca.jianghu66.top

[R49] awk 带条件
来源：http://wiw.gotoacloud.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dxz.yj20258888.top

[R50] awk 求和
来源：http://hzb.gaohongyu789.top

awk '{s += $2} END {print s}' a.txt
来源：http://cjv.zhijiandao.cn

[R51] 排序去重取前几
来源：http://bkd.shanyushiyangkeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://cgc.yanxiufei.cn

[R52] 统计行数
来源：http://anz.nwbrower.top

wc -l a.txt
来源：http://qcy.haohaochexian.top

[R53] 查看文件头与实时尾
来源：http://qoi.shanyushiyangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hjb.kuanghao11.cn

[R54] 比较两个文件
来源：http://nal.yuanzhike.top

diff a.txt b.txt
来源：http://ifo.epnwcf.com

[R55] 压缩与解压
来源：http://jvc.fengsongda.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fqc.havefunace.top

[R56] 远程拷贝
来源：http://srz.hesvh.cn

scp file user@host:/path/
来源：http://fhm.bjfxy.top

[R57] 远程执行命令
来源：http://gcp.gogol.net.cn

ssh user@host 'uptime'
来源：http://ckr.pengpengdd.cyou

[R58] 下载文件
来源：http://ozs.sufxvd.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yjs.hammf.cn

[R59] 发 POST JSON
来源：http://cjy.cdnleiting.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lyh.sysykeji.top

[R60] 只看 HTTP 状态码
来源：http://qdq.316326.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uwd.hnxiangtu.top

[R61] 磁盘占用
来源：http://oco.fengsongda.top

df -h;  du -sh *
来源：http://yyq.feifeiyinyue.top

[R62] 找最占空间的文件
来源：http://knk.tianlin.xyz

du -ah . | sort -rh | head -10
来源：http://xav.zhiwuduotai.top

[R63] 内存与进程
来源：http://npg.wangdashe.top

free -h;  ps aux | grep nginx
来源：http://ilk.zhixingplan.top

[R64] 结束进程
来源：http://lwt.hfpthk.cn

kill -9 $(pgrep -f app.py)
来源：http://zib.yanxiufei.cn

[R65] 查看端口占用
来源：http://biu.jlsjyb.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://egr.yvedp.cn

[R66] 定时任务
来源：http://yon.xuanzx.com

crontab -e;  crontab -l
来源：http://lwa.jqgfzy.top

[R67] 生成随机十六进制串
来源：http://okp.ywan-chungtsiang.top

openssl rand -hex 16
来源：http://zmx.yueranfly.top

[R68] 计算文件校验值
来源：http://ybn.sjlbkw.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vvr.kuanghao11.cn

[R69] 生成随机密码
来源：http://kxz.fehbvm.com

head -c 16 /dev/urandom | base64
来源：http://ncw.hcnkem.com

[R70] 时间戳与互转
来源：http://gxa.chenjidiqi.icu

date +%s;  date -d @1700000000
来源：http://zfv.sweek.top

[R71] 日期格式化
来源：http://xpb.iojbl.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wjv.xinyue.icu

[R72] 等待端口就绪
来源：http://lzg.nanxinkj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qet.redwolf501.top

[R73] 分割大日志
来源：http://uud.gaohongyu789.top

split -l 1000 big.log part_
来源：http://zgk.xziqi.cn

[R74] 批量重命名
来源：http://htl.quarkkingdee.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bhc.mhx1999.top

[R75] 导出环境变量
来源：http://ifw.shzxlz.cn

export PATH="$HOME/bin:$PATH"
来源：http://bcp.gogol.net.cn

[R76] 使用临时文件
来源：http://ziv.9152youxi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vub.hnqzz.top

[R77] 读取用户输入
来源：http://icy.ydjk.org.cn

read -rp "请输入: " ans
来源：http://chj.hongshengwenyu.top

[R78] 交互式菜单
来源：http://ufv.redwolf501.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ngq.ywan-chungtsiang.top

[R79] 解析命令行选项
来源：http://jug.zhixingplan.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jbp.birdmap.top

[R80] 查看脚本执行耗时
来源：http://jtn.0kj1m.cn

time ./run.sh
来源：http://awu.ydjk.org.cn

================================================================================
来源：http://yfy.hnxiangtu.top

S. C / C++ 专题
来源：http://wzr.gzhubu.top

================================================================================
来源：http://wyz.meibo888.top

[S01] C：Hello World
来源：http://rdc.jinghuilouyu.cn

#include <stdio.h>
来源：http://mse.pengpengdd.cyou

int main(void) { printf("Hello\n"); return 0; }
来源：http://gnv.guowangkeji.top

[S02] C：变量与格式化输出
来源：http://erg.jqgufenzy.top

int a = 10; printf("%d\n", a);
来源：http://rht.xuanzx.com

[S03] C：读入整数
来源：http://kju.tanke756.top

int x; scanf("%d", &x);
来源：http://ney.yj20258888.top

[S04] C：字符串复制
来源：http://qrr.jinqigfzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://fwi.wangshuangyany.cn

[S05] C：字符串长度
来源：http://zvi.fanxiaobao.xyz

strlen(s)
来源：http://vsr.dianchejie.cn

[S06] C：字符串比较
来源：http://xfm.redwolf501.top

strcmp(a, b) == 0
来源：http://wkb.jinghuilouyu.cn

[S07] C：数组遍历求和
来源：http://rut.sweek.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ird.ydzc1.top

[S08] C：动态内存分配与释放
来源：http://czk.yvedp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cmq.hywenlv.cn

[S09] C：结构体定义与初始化
来源：http://jbv.shanyushiyangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vke.jinqigfzy.top

[S10] C：指针与解引用
来源：http://ght.ppjwa.cn

int *p = &a;  *p = 5;
来源：http://yso.yueranfly.top

[S11] C：逐行读文件
来源：http://wcy.vqdsnc.cn

FILE *f = fopen("a.txt", "r");
来源：http://omy.epnwcf.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://dxl.daria6918.cn

fclose(f);
来源：http://mlc.yj202588.top

[S12] C：写文件
来源：http://tve.smart0.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zpa.ywan-chungtsiang.top

[S13] C：宏定义
来源：http://smm.ydjk.org.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qcv.uphjek.com

[S14] C：枚举
来源：http://qho.shzxlz.cn

enum Color { RED, GREEN, BLUE };
来源：http://hms.chenjidiqi.icu

[S15] C：类型转换
来源：http://pcl.xziqi.cn

(double) a / b
来源：http://hkp.hnqzz.top

[S16] C：位操作置位
来源：http://rfe.sysykeji.top

x |= (1 << 3);
来源：http://xgd.9152youxi.cn

[S17] C：安全拼接字符串
来源：http://bvs.zhiwuduotai.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://civ.nanxuanxn.top

[S18] C：命令行参数
来源：http://dfv.sysykeji.top

int main(int argc, char **argv)
来源：http://gxm.0kj1m.cn

[S19] C：快速排序
来源：http://agz.tanke756.top

qsort(a, n, sizeof(int), cmp);
来源：http://nod.cqqwz.cn

[S20] C：二分查找
来源：http://myr.hysaishi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sst.yvedp.cn

[S21] C：字符类别判断
来源：http://aaw.chenjidiqi.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fhi.hesvh.cn

[S22] C：字符串转数字
来源：http://djp.zhoulong.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://buc.sufxvd.cn

[S23] C：随机数
来源：http://pch.zycfv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nae.zhoulong.xyz

[S24] C：获取本地时间
来源：http://irw.xingfuxueyuan.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zam.zdqjudy.top

[S25] C：内存拷贝
来源：http://rrm.bjfxy.top

memcpy(dst, src, n);
来源：http://swf.bbcook.cn

[S26] C：内存清零
来源：http://csy.shangyingyoupin.top

memset(a, 0, sizeof a);
来源：http://mhx.wangdashe.top

[S27] C：定义常量
来源：http://hna.jiagoushi.top

const double PI = 3.14159;
来源：http://zzl.guannengcc.top

[S28] C：静态变量
来源：http://qwy.ctjpmb.com

static int counter = 0;
来源：http://xfz.jinqigufen.top

[S29] C：变参函数
来源：http://dnf.iojbl.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kca.xziqi.cn

[S30] C：头文件保护
来源：http://jvl.havefunace.top

#ifndef X_H
来源：http://kar.chenzaomai.com

#define X_H
来源：http://jch.jinqigfzy.top

#endif
来源：http://dzs.jqgufenzy.top

[S31] C++：Hello World
来源：http://byb.jlsjyb.cn

#include <iostream>
来源：http://scm.jinyuanbaomall.cn

int main() { std::cout << "Hello\n"; }
来源：http://eyj.sufxvd.cn

[S32] C++：字符串
来源：http://apz.uphjek.com

std::string s = "hi";  s += "!";
来源：http://ikd.0kj1m.cn

[S33] C++：vector 增删
来源：http://xaj.haohaochexian.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vsn.dashuyun.cn

[S34] C++：遍历 vector
来源：http://llc.gotoacloud.top

for (auto &x : v) { std::cout << x; }
来源：http://xfv.ivvv.top

[S35] C++：map
来源：http://ezk.zhengqikj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cnb.jinghuilouyu.cn

[S36] C++：unordered_map
来源：http://gty.yanxiufei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xvb.hammf.cn

[S37] C++：set
来源：http://rcd.yanxiufei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zqz.zhoulong.xyz

[S38] C++：排序
来源：http://lzl.dianchejie.cn

std::sort(v.begin(), v.end());
来源：http://irm.hongshengwenyu.top

[S39] C++：自定义比较器排序
来源：http://hlb.shzxlz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gkg.chenzaomai.com

[S40] C++：查找元素
来源：http://mrb.hnxiangtu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://iym.xuetiantiany.cn

[S41] C++：类与构造函数
来源：http://mwe.nanxinkj.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vxv.cashguo.top

[S42] C++：继承与虚函数
来源：http://dsq.xuetiantiany.cn

class B : public Base { public: void f() override {} };
来源：http://jty.cqqwz.cn

[S43] C++：智能指针
来源：http://ueb.yuxming.cn

auto p = std::make_unique<int>(5);
来源：http://euw.hysaishi.cn

[S44] C++：引用传参
来源：http://nra.vqdsnc.cn

void inc(int &x) { ++x; }
来源：http://dbv.hongshengwenyu.top

[S45] C++：lambda
来源：http://kyw.jiagoushi.top

auto add = [](int a, int b) { return a + b; };
来源：http://usm.ppjwa.cn

[S46] C++：函数模板
来源：http://mkh.chenlongwang.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zdg.chenjidiqi.icu


<!-- 参考信息 -->