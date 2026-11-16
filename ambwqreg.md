代发 wailian999

[Q82] 字符长度与字节长度
来源：http://bgc.gotoacloud.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rfr.cdnleiting.top

[Q83] 大小写转换
来源：http://lvx.cheryme.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cpc.bjfxy.top

[Q84] 去除首尾空格
来源：http://eof.zhixingplan.top

SELECT TRIM(name) FROM users;
来源：http://wad.zdbjq.cn

[Q85] 数值取整
来源：http://bhk.zycfv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rxu.wangdashe.top

[Q86] 读取 JSON 字段
来源：http://drp.ydjk.org.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://piq.zdbjq.cn

[Q87] JSON 字段做条件
来源：http://ocj.mhx1999.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wdi.zhiwuduotai.top

[Q88] 行转列（条件聚合）
来源：http://zmr.hnxiangtu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yvm.aizwys.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://epr.nanxinkj.top

[Q89] 判断表是否存在
来源：http://tol.guowangkeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ppo.guannengcc.top

[Q90] 生成序号列
来源：http://nfh.yuanzhike.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lki.pycfn.com

================================================================================
来源：http://bzx.aibaodan.cn

R. Bash 专题
来源：http://rmp.zhoulong.xyz

================================================================================
来源：http://frb.yj202588.top

[R01] shebang 与严格模式
来源：http://tls.yongpay.top

#!/usr/bin/env bash
来源：http://rda.xylfe.cn

set -euo pipefail
来源：http://ugh.feifeiyinyue.top

[R02] 变量赋值与使用
来源：http://omf.wangshuangyany.cn

name="Tom"; echo "$name"
来源：http://lvt.bjfxy.top

[R03] 只读变量
来源：http://bhx.bbcook.cn

readonly PI=3.14
来源：http://uea.cheryme.top

[R04] 位置参数
来源：http://fmu.cdnleiting.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wqd.kuanghao11.cn

[R05] 参数默认值
来源：http://kec.316326.xyz

name="${1:-default}"
来源：http://zcf.nanxuanxn.top

[R06] 判断命令是否存在
来源：http://rij.cucudq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rtl.zhijiandao.cn

[R07] if 判断文件
来源：http://qjd.feifeiyinyue.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wmd.hywenlv.cn

[R08] 数值比较
来源：http://cev.jyoumei.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pud.dianchejie.cn

[R09] 字符串比较
来源：http://qni.jinghuilouyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://smw.daxiang520.top

[R10] 正则匹配
来源：http://egd.shzxlz.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zus.yonumen.top

[R11] case 多分支
来源：http://iqg.zhiwuduotai.top

case "$1" in
来源：http://uvu.bbcook.cn

start) echo "启动" ;;
来源：http://epu.tanke756.top

stop)  echo "停止" ;;
来源：http://pmw.jinqigufen.top

*)     echo "未知命令" ;;
来源：http://qix.zhiwuduotai.top

esac
来源：http://eqx.hongshengwenyu.top

[R12] for 遍历文件
来源：http://xfn.uphjek.com

for f in *.txt; do echo "$f"; done
来源：http://jow.shzxlz.cn

[R13] for 计数循环
来源：http://tru.cashguo.top

for i in {1..10}; do echo "$i"; done
来源：http://fwd.ctjpmb.com

[R14] C 风格 for
来源：http://nsa.guannengcc.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ctf.aibaodan.cn

[R15] while 逐行读文件
来源：http://mcn.jlsjyb.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yak.iojbl.cn

[R16] until 等待条件
来源：http://cbx.hnqzz.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ybp.tianlin.xyz

[R17] 数组定义与取值
来源：http://cgr.ivvv.top

arr=(a b c); echo "${arr[0]}"
来源：http://jkl.gaohongyu789.top

[R18] 遍历数组
来源：http://svm.cashguo.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fxe.shzxlz.cn

[R19] 数组长度
来源：http://sbr.meibo888.top

echo "${#arr[@]}"
来源：http://ukr.svipenyu.cn

[R20] 关联数组（字典）
来源：http://pfd.cdnleiting.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://olk.fehbvm.com

[R21] 字符串长度
来源：http://ffj.zhiwuduotai.top

echo "${#s}"
来源：http://ujh.ppjwa.cn

[R22] 截取子串
来源：http://snp.uphjek.com

echo "${s:0:5}"
来源：http://wim.hammf.cn

[R23] 字符串替换
来源：http://tbw.shangyingyoupin.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gey.daxiang520.top

[R24] 大小写转换
来源：http://iog.xziqi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yfz.haohaochexian.top

[R25] 去后缀 / 去前缀
来源：http://wny.ywan-chungtsiang.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://uji.cucudq.cn

[R26] 命令替换
来源：http://hza.haohaochexian.top

now=$(date +%F); echo "$now"
来源：http://wvs.ctjpmb.com

[R27] 算术展开
来源：http://llt.wangshuangyany.cn

echo $((1 + 2 * 3))
来源：http://eij.zhoulong.xyz

[R28] 浮点运算
来源：http://qqe.haohaochexian.top

echo "scale=2; 10/3" | bc
来源：http://cae.ivvv.top

[R29] 定义函数
来源：http://ppk.epnwcf.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fim.fzhhl.top

[R30] 函数返回状态码
来源：http://rwn.fengsongda.top

f() { return 0; }; f || echo "失败了"
来源：http://sxb.pengpengdd.cyou

[R31] 局部变量
来源：http://yye.jinqigufen.top

f() { local x=1; echo "$x"; }
来源：http://sgs.zycfv.cn

[R32] 参数个数校验
来源：http://mlz.cucudq.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sqs.quarkkingdee.top

[R33] 捕获错误并提示行号
来源：http://vtj.chenjidiqi.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hef.vqdsnc.cn

[R34] 退出时清理
来源：http://idb.epnwcf.com

trap 'rm -f "$tmp"' EXIT
来源：http://azq.jqgfzy.top

[R35] 后台执行并等待
来源：http://eur.chenjidiqi.icu

sleep 5 & pid=$!; wait "$pid"
来源：http://mjz.nwbrower.top

[R36] 并发执行多个任务
来源：http://vkt.hammf.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gyt.daxiang520.top

[R37] 把输出赋给变量
来源：http://gnl.guannengcc.top

files=$(ls -1)
来源：http://cxy.xingfuxueyuan.xyz

[R38] 管道串联
来源：http://ctc.chenjidiqi.icu

cat a.txt | grep -i error | wc -l
来源：http://lmd.sjlbkw.cn

[R39] 重定向标准输出与错误
来源：http://rao.yfazqb.com

cmd > out.log 2>&1
来源：http://kjl.gaohongyu789.top

[R40] 追加写日志
来源：http://nvx.ydzc1.top

echo "log" >> out.log
来源：http://dng.fanxiaobao.xyz

[R41] 丢弃输出
来源：http://uns.316326.xyz

cmd >/dev/null 2>&1
来源：http://bvf.shzxlz.cn

[R42] 输入重定向
来源：http://mld.shanyushiyangkeji.top

wc -l < a.txt
来源：http://jwp.ydjk.org.cn

[R43] 按名字查找文件
来源：http://hlb.tianlin.xyz

find . -name "*.log" -type f
来源：http://bwh.hammf.cn

[R44] 按修改时间查找
来源：http://svy.gogol.net.cn

find . -mtime -7 -type f
来源：http://iok.zhiwuduotai.top

[R45] 批量删除
来源：http://kea.nanxinkj.top

find . -name "*.tmp" -delete
来源：http://zgr.ivvv.top

[R46] 递归替换文件内容
来源：http://ijs.zhiwuduotai.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://okk.kuanghao11.cn

[R47] sed 单行替换
来源：http://wuq.hywenlv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xzi.vqdsnc.cn

[R48] awk 取指定列
来源：http://sxb.snrcjt.cn

awk '{print $1, $3}' a.txt
来源：http://itq.zhiwuduotai.top

[R49] awk 带条件
来源：http://ybv.guannengcc.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nsw.jinqigfzy.top

[R50] awk 求和
来源：http://ply.zdbjq.cn

awk '{s += $2} END {print s}' a.txt
来源：http://raz.yvedp.cn

[R51] 排序去重取前几
来源：http://zeq.gaohongyu789.top

sort a.txt | uniq -c | sort -rn | head
来源：http://dxh.fktsv.cn

[R52] 统计行数
来源：http://rlc.gotoacloud.top

wc -l a.txt
来源：http://and.zycfv.cn

[R53] 查看文件头与实时尾
来源：http://lua.yj202588.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jna.yuanzhike.top

[R54] 比较两个文件
来源：http://sxr.hcnkem.com

diff a.txt b.txt
来源：http://omx.jiagoushi.top

[R55] 压缩与解压
来源：http://bcr.hcnkem.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tje.aibaodan.cn

[R56] 远程拷贝
来源：http://lky.epnwcf.com

scp file user@host:/path/
来源：http://oxi.epnwcf.com

[R57] 远程执行命令
来源：http://hwk.sweek.top

ssh user@host 'uptime'
来源：http://eza.fktsv.cn

[R58] 下载文件
来源：http://ztn.chenlongwang.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ves.daxiang520.top

[R59] 发 POST JSON
来源：http://hqt.zhongyouzk.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://orq.bjfxy.top

[R60] 只看 HTTP 状态码
来源：http://djk.sxryk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://crd.cashguo.top

[R61] 磁盘占用
来源：http://xok.tian-w.cn

df -h;  du -sh *
来源：http://nbj.yfazqb.com

[R62] 找最占空间的文件
来源：http://dvg.vehdjk.com

du -ah . | sort -rh | head -10
来源：http://bxv.andypj.xyz

[R63] 内存与进程
来源：http://zgy.guannengcc.top

free -h;  ps aux | grep nginx
来源：http://omi.jinqigufen.top

[R64] 结束进程
来源：http://wei.shangyingyoupin.top

kill -9 $(pgrep -f app.py)
来源：http://nvj.guannengcc.top

[R65] 查看端口占用
来源：http://qmb.yj202588.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ppj.iojbl.cn

[R66] 定时任务
来源：http://dxc.sufxvd.cn

crontab -e;  crontab -l
来源：http://yxd.mhx1999.top

[R67] 生成随机十六进制串
来源：http://okn.hongshengwenyu.top

openssl rand -hex 16
来源：http://ccn.fanxiaobao.xyz

[R68] 计算文件校验值
来源：http://zxl.cashguo.top

sha256sum a.txt;  md5sum a.txt
来源：http://zcs.andypj.xyz

[R69] 生成随机密码
来源：http://rjs.ydzc1.top

head -c 16 /dev/urandom | base64
来源：http://rca.zycfv.cn

[R70] 时间戳与互转
来源：http://bml.tanke756.top

date +%s;  date -d @1700000000
来源：http://qbr.birdmap.top

[R71] 日期格式化
来源：http://ipn.zhongyouzk.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://oou.pycfn.com

[R72] 等待端口就绪
来源：http://sur.yonumen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ocg.guannengcc.top

[R73] 分割大日志
来源：http://uym.zycfv.cn

split -l 1000 big.log part_
来源：http://ptj.yj20258.top

[R74] 批量重命名
来源：http://dbb.hywenlv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tvk.tanke756.top

[R75] 导出环境变量
来源：http://cyn.aizwys.cn

export PATH="$HOME/bin:$PATH"
来源：http://jvt.ywan-chungtsiang.top

[R76] 使用临时文件
来源：http://qax.cucudq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fht.xingfuxueyuan.xyz

[R77] 读取用户输入
来源：http://fjd.kuanghao11.cn

read -rp "请输入: " ans
来源：http://awx.smart0.xyz

[R78] 交互式菜单
来源：http://edr.birdmap.top

select opt in a b c; do echo "$opt"; break; done
来源：http://fld.shanyushiyangkeji.top

[R79] 解析命令行选项
来源：http://nyb.dashuyun.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tpj.9152youxi.cn

[R80] 查看脚本执行耗时
来源：http://lah.yj20258888.top

time ./run.sh
来源：http://xuo.nanxinkj.top

================================================================================
来源：http://ezi.dianchejie.cn

S. C / C++ 专题
来源：http://ewi.havefunace.top

================================================================================
来源：http://jlk.sweek.top

[S01] C：Hello World
来源：http://tft.ybcxt.top

#include <stdio.h>
来源：http://drk.zhiwuduotai.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://trg.hongshengwenyu.top

[S02] C：变量与格式化输出
来源：http://mop.quarkkingdee.top

int a = 10; printf("%d\n", a);
来源：http://xhc.sysykeji.top

[S03] C：读入整数
来源：http://tls.zhixingplan.top

int x; scanf("%d", &x);
来源：http://rsp.mhx1999.top

[S04] C：字符串复制
来源：http://rgc.haohaochexian.top

char dst[32]; strcpy(dst, "hi");
来源：http://ehn.yongpay.top

[S05] C：字符串长度
来源：http://yjx.jinqigfzy.top

strlen(s)
来源：http://jdi.dianchejie.cn

[S06] C：字符串比较
来源：http://ubj.jinghuilouyu.cn

strcmp(a, b) == 0
来源：http://aow.yanxiufei.cn

[S07] C：数组遍历求和
来源：http://dco.andypj.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ngy.haohaochexian.top

[S08] C：动态内存分配与释放
来源：http://qdc.pengpengdd.cyou

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qyx.yongpay.top

[S09] C：结构体定义与初始化
来源：http://syz.jinqigufen.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dks.vehdjk.com

[S10] C：指针与解引用
来源：http://ndg.ctjpmb.com

int *p = &a;  *p = 5;
来源：http://ytj.9152youxi.cn

[S11] C：逐行读文件
来源：http://uyz.shangyingyoupin.top

FILE *f = fopen("a.txt", "r");
来源：http://dlj.tian-w.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://erl.uphjek.com

fclose(f);
来源：http://fou.ydzc1.top

[S12] C：写文件
来源：http://mtj.yuanzhike.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ojf.wangshuangyany.cn

[S13] C：宏定义
来源：http://bid.jinqigufen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://czl.fehbvm.com

[S14] C：枚举
来源：http://efm.bbcook.cn

enum Color { RED, GREEN, BLUE };
来源：http://rkf.hywenlv.cn

[S15] C：类型转换
来源：http://fnp.zhaomingkeji.xyz

(double) a / b
来源：http://vep.hesvh.cn

[S16] C：位操作置位
来源：http://htb.hnqzz.top

x |= (1 << 3);
来源：http://dti.gaohongyu789.top

[S17] C：安全拼接字符串
来源：http://ymo.yangfankeji.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hfu.chenjidiqi.icu

[S18] C：命令行参数
来源：http://itx.gaohongyu789.top

int main(int argc, char **argv)
来源：http://nti.zdbjq.cn

[S19] C：快速排序
来源：http://pwp.zhongyouzk.top

qsort(a, n, sizeof(int), cmp);
来源：http://mri.havefunace.top

[S20] C：二分查找
来源：http://rmr.zdqjudy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://isp.tanke756.top

[S21] C：字符类别判断
来源：http://dwc.xziqi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://egb.ivvv.top

[S22] C：字符串转数字
来源：http://het.ydjk.org.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gtu.hnqzz.top

[S23] C：随机数
来源：http://pqe.ctjpmb.com

srand(time(NULL));  int r = rand() % 100;
来源：http://gby.ydzc1.top

[S24] C：获取本地时间
来源：http://uzl.316326.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xjz.52xcode.cn

[S25] C：内存拷贝
来源：http://ezm.tian-w.cn

memcpy(dst, src, n);
来源：http://viu.bjfxy.top

[S26] C：内存清零
来源：http://bqh.feifeiyinyue.top

memset(a, 0, sizeof a);
来源：http://zyd.sufxvd.cn

[S27] C：定义常量
来源：http://fsd.zycfv.cn

const double PI = 3.14159;
来源：http://msu.vehdjk.com

[S28] C：静态变量
来源：http://auu.xinyue.icu

static int counter = 0;
来源：http://exb.yanxiufei.cn

[S29] C：变参函数
来源：http://bem.birdmap.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pnv.guannengcc.top

[S30] C：头文件保护
来源：http://uip.xingfuxueyuan.xyz

#ifndef X_H
来源：http://txl.316326.xyz

#define X_H
来源：http://ixi.fengsongda.top

#endif
来源：http://bdk.ivvv.top

[S31] C++：Hello World
来源：http://bqt.ctjpmb.com

#include <iostream>
来源：http://bxj.zhoulong.xyz

int main() { std::cout << "Hello\n"; }
来源：http://gzr.sufxvd.cn

[S32] C++：字符串
来源：http://lgx.gaohongyu789.top

std::string s = "hi";  s += "!";
来源：http://rtq.ivvv.top

[S33] C++：vector 增删
来源：http://lgg.redwolf501.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sua.fengsongda.top

[S34] C++：遍历 vector
来源：http://xsp.zdbjq.cn

for (auto &x : v) { std::cout << x; }
来源：http://qmk.wangshuangyany.cn

[S35] C++：map
来源：http://zcf.jqgfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yuu.nanxinkj.top

[S36] C++：unordered_map
来源：http://fgr.yuanzhike.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://oqx.hnqzz.top

[S37] C++：set
来源：http://lka.yangfankeji.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qjk.quarkkingdee.top

[S38] C++：排序
来源：http://ryu.cucudq.cn

std::sort(v.begin(), v.end());
来源：http://bzp.jyoumei.cn

[S39] C++：自定义比较器排序
来源：http://xag.aizwys.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lgq.pycfn.com

[S40] C++：查找元素
来源：http://qmy.ybcxt.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cmu.xinyue.icu

[S41] C++：类与构造函数
来源：http://jhu.yangfankeji.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lfo.xinyue.icu

[S42] C++：继承与虚函数
来源：http://lcr.bjfxy.top

class B : public Base { public: void f() override {} };
来源：http://jye.hcnkem.com

[S43] C++：智能指针
来源：http://caq.aizwys.cn

auto p = std::make_unique<int>(5);
来源：http://xto.guannengcc.top

[S44] C++：引用传参
来源：http://tqb.meibo888.top

void inc(int &x) { ++x; }
来源：http://xin.meibo888.top

[S45] C++：lambda
来源：http://dtm.sufxvd.cn

auto add = [](int a, int b) { return a + b; };
来源：http://svx.tian-w.cn

[S46] C++：函数模板
来源：http://nxv.nwbrower.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ozk.havefunace.top

[S47] C++：结构化绑定遍历
来源：http://xch.hammf.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://aey.fktsv.cn

[S48] C++：逐行读文件
来源：http://rch.hysaishi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://baw.fengsongda.top

while (std::getline(in, line)) { }
来源：http://syc.tarul.cn

[S49] C++：写文件
来源：http://fzs.kuanghao11.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ukl.wangshuangyany.cn

[S50] C++：格式化数字
来源：http://ecv.tanke756.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ybq.aizwys.cn

[S51] C++：显式类型转换
来源：http://rym.ydjk.org.cn

static_cast<double>(a) / b
来源：http://rat.zhiwuduotai.top

[S52] C++：const 与 noexcept
来源：http://tbp.zhongyouzk.top


<!-- 参考信息 -->