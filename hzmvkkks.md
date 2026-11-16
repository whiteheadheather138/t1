代发 wailian999

[Q86] 读取 JSON 字段
来源：http://kyk.hcnkem.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hix.yanxiufei.cn

[Q87] JSON 字段做条件
来源：http://btg.sysykeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oqf.cqqwz.cn

[Q88] 行转列（条件聚合）
来源：http://ehe.jiagoushi.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qxi.jianghu66.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gvh.yj20258888.top

[Q89] 判断表是否存在
来源：http://tih.shanyushiyangkeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xjf.yanxiufei.cn

[Q90] 生成序号列
来源：http://fad.birdmap.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hak.jinqigufen.top

================================================================================
来源：http://upj.zhijiandao.cn

R. Bash 专题
来源：http://bhm.yangfankeji.com

================================================================================
来源：http://zhu.snrcjt.cn

[R01] shebang 与严格模式
来源：http://bxa.yonumen.top

#!/usr/bin/env bash
来源：http://vcb.ywan-chungtsiang.top

set -euo pipefail
来源：http://zrc.c1oappe.top

[R02] 变量赋值与使用
来源：http://fqu.sweek.top

name="Tom"; echo "$name"
来源：http://fom.jlsjyb.cn

[R03] 只读变量
来源：http://fmb.dashuyun.cn

readonly PI=3.14
来源：http://epb.yfazqb.com

[R04] 位置参数
来源：http://lsk.xuetiantiany.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jvk.epnwcf.com

[R05] 参数默认值
来源：http://eam.zhaomingkeji.xyz

name="${1:-default}"
来源：http://tjn.bbcook.cn

[R06] 判断命令是否存在
来源：http://nuy.bjfxy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nju.yuxming.cn

[R07] if 判断文件
来源：http://nnb.wangdashe.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://stl.jianghu66.top

[R08] 数值比较
来源：http://gls.tarul.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bia.jqgfzy.top

[R09] 字符串比较
来源：http://yyh.wangshuangyany.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ney.hfpthk.cn

[R10] 正则匹配
来源：http://cif.hysaishi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://aja.snrcjt.cn

[R11] case 多分支
来源：http://til.sxryk.cn

case "$1" in
来源：http://yvw.birdmap.top

start) echo "启动" ;;
来源：http://thc.gaohongyu789.top

stop)  echo "停止" ;;
来源：http://nxd.0kj1m.cn

*)     echo "未知命令" ;;
来源：http://eba.zycfv.cn

esac
来源：http://vnj.xylfe.cn

[R12] for 遍历文件
来源：http://gxk.nanxinkj.top

for f in *.txt; do echo "$f"; done
来源：http://svm.c1oappe.top

[R13] for 计数循环
来源：http://epu.hnqzz.top

for i in {1..10}; do echo "$i"; done
来源：http://bsn.shanyushiyangtech.top

[R14] C 风格 for
来源：http://dbn.vehdjk.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kjh.tianlin.xyz

[R15] while 逐行读文件
来源：http://gzv.nwbrower.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://peo.yfazqb.com

[R16] until 等待条件
来源：http://thj.zhixingplan.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rcw.yj202588.top

[R17] 数组定义与取值
来源：http://djx.gotoacloud.top

arr=(a b c); echo "${arr[0]}"
来源：http://ivu.hfpthk.cn

[R18] 遍历数组
来源：http://eit.ehwqpu.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zzk.zdqjudy.top

[R19] 数组长度
来源：http://ors.bbcook.cn

echo "${#arr[@]}"
来源：http://bsi.jiagoushi.top

[R20] 关联数组（字典）
来源：http://hpr.hcnkem.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kux.nanxinkj.top

[R21] 字符串长度
来源：http://qmp.hammf.cn

echo "${#s}"
来源：http://zcc.haohaochexian.top

[R22] 截取子串
来源：http://hgh.zhixingplan.top

echo "${s:0:5}"
来源：http://xks.hongshengwenyu.top

[R23] 字符串替换
来源：http://yxi.yuanzhike.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sii.zhaomingkeji.xyz

[R24] 大小写转换
来源：http://pnn.gzhubu.top

echo "${s^^}"; echo "${s,,}"
来源：http://bod.zhijiandao.cn

[R25] 去后缀 / 去前缀
来源：http://spm.feifeiyinyue.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://gen.smart0.xyz

[R26] 命令替换
来源：http://oxp.sjlbkw.cn

now=$(date +%F); echo "$now"
来源：http://oyb.jinghuilouyu.cn

[R27] 算术展开
来源：http://hpr.yueranfly.top

echo $((1 + 2 * 3))
来源：http://fuj.mhx1999.top

[R28] 浮点运算
来源：http://jhr.pycfn.com

echo "scale=2; 10/3" | bc
来源：http://aux.hnqzz.top

[R29] 定义函数
来源：http://joa.shanyushiyangtech.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ypb.vehdjk.com

[R30] 函数返回状态码
来源：http://xvp.yj20258.top

f() { return 0; }; f || echo "失败了"
来源：http://cbq.jqgufenzy.top

[R31] 局部变量
来源：http://upx.jlsjyb.cn

f() { local x=1; echo "$x"; }
来源：http://vav.zhongyouzk.top

[R32] 参数个数校验
来源：http://lig.zdbjq.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lxl.aibaodan.cn

[R33] 捕获错误并提示行号
来源：http://wmo.kuanghao11.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://esn.sxryk.cn

[R34] 退出时清理
来源：http://kkp.ivvv.top

trap 'rm -f "$tmp"' EXIT
来源：http://htj.jyoumei.cn

[R35] 后台执行并等待
来源：http://jxy.jinqigufen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://zwa.yvedp.cn

[R36] 并发执行多个任务
来源：http://pdp.chenzaomai.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://poq.xuanzx.com

[R37] 把输出赋给变量
来源：http://dgw.gogol.net.cn

files=$(ls -1)
来源：http://wdc.guowangkeji.top

[R38] 管道串联
来源：http://wlv.nwbrower.top

cat a.txt | grep -i error | wc -l
来源：http://fjl.uphjek.com

[R39] 重定向标准输出与错误
来源：http://fum.shanyushiyangtech.top

cmd > out.log 2>&1
来源：http://jfh.smart0.xyz

[R40] 追加写日志
来源：http://brr.epnwcf.com

echo "log" >> out.log
来源：http://ril.hysaishi.cn

[R41] 丢弃输出
来源：http://kde.yj20258.top

cmd >/dev/null 2>&1
来源：http://xiq.fengsongda.top

[R42] 输入重定向
来源：http://ufq.cdnleiting.top

wc -l < a.txt
来源：http://gfx.haohaochexian.top

[R43] 按名字查找文件
来源：http://sub.aizwys.cn

find . -name "*.log" -type f
来源：http://epu.jinqigufen.top

[R44] 按修改时间查找
来源：http://fwb.cqqwz.cn

find . -mtime -7 -type f
来源：http://gma.hywenlv.cn

[R45] 批量删除
来源：http://fyo.jinqigufen.top

find . -name "*.tmp" -delete
来源：http://dcg.wangshuangyany.cn

[R46] 递归替换文件内容
来源：http://ubz.dianchejie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ujw.xuetiantiany.cn

[R47] sed 单行替换
来源：http://okr.fzhhl.top

sed -i 's/foo/bar/g' a.txt
来源：http://gmu.yfazqb.com

[R48] awk 取指定列
来源：http://bls.tianlin.xyz

awk '{print $1, $3}' a.txt
来源：http://bel.hongshengwenyu.top

[R49] awk 带条件
来源：http://hqv.mhx1999.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cxo.9152youxi.cn

[R50] awk 求和
来源：http://gah.9152youxi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bca.nwbrower.top

[R51] 排序去重取前几
来源：http://ume.tarul.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gdt.vqdsnc.cn

[R52] 统计行数
来源：http://ewl.ppjwa.cn

wc -l a.txt
来源：http://rqd.fktsv.cn

[R53] 查看文件头与实时尾
来源：http://sxm.hnqzz.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://aav.52xcode.cn

[R54] 比较两个文件
来源：http://fwr.cucudq.cn

diff a.txt b.txt
来源：http://jcl.chenzaomai.com

[R55] 压缩与解压
来源：http://tpv.zhongyouzk.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mxk.aibaodan.cn

[R56] 远程拷贝
来源：http://cbv.havefunace.top

scp file user@host:/path/
来源：http://kbg.zhijiandao.cn

[R57] 远程执行命令
来源：http://diq.cdnleiting.top

ssh user@host 'uptime'
来源：http://yqx.redwolf501.top

[R58] 下载文件
来源：http://izb.sjlbkw.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cmh.sufxvd.cn

[R59] 发 POST JSON
来源：http://kjo.aibaodan.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zsg.shanyushiyangtech.top

[R60] 只看 HTTP 状态码
来源：http://evw.gaohongyu789.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://spv.fengsongda.top

[R61] 磁盘占用
来源：http://wcb.zhixingplan.top

df -h;  du -sh *
来源：http://bfb.redwolf501.top

[R62] 找最占空间的文件
来源：http://jpa.jinqigufen.top

du -ah . | sort -rh | head -10
来源：http://fnn.sysykeji.top

[R63] 内存与进程
来源：http://jam.fktsv.cn

free -h;  ps aux | grep nginx
来源：http://vtf.yj20258.top

[R64] 结束进程
来源：http://fou.pycfn.com

kill -9 $(pgrep -f app.py)
来源：http://gce.ehwqpu.com

[R65] 查看端口占用
来源：http://ajr.jinyuanbaomall.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hdd.jinqigfzy.top

[R66] 定时任务
来源：http://jnn.zhongyouzk.top

crontab -e;  crontab -l
来源：http://yqn.zhaomingkeji.xyz

[R67] 生成随机十六进制串
来源：http://yiv.zhongyouzk.top

openssl rand -hex 16
来源：http://kat.fehbvm.com

[R68] 计算文件校验值
来源：http://ywn.cqqwz.cn

sha256sum a.txt;  md5sum a.txt
来源：http://twk.yongpay.top

[R69] 生成随机密码
来源：http://xuw.guannengcc.top

head -c 16 /dev/urandom | base64
来源：http://gxu.hysaishi.cn

[R70] 时间戳与互转
来源：http://tpw.fktsv.cn

date +%s;  date -d @1700000000
来源：http://oad.iojbl.cn

[R71] 日期格式化
来源：http://avj.jyoumei.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gpz.guowangkeji.top

[R72] 等待端口就绪
来源：http://vet.dashuyun.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fab.sufxvd.cn

[R73] 分割大日志
来源：http://svm.havefunace.top

split -l 1000 big.log part_
来源：http://xsr.epnwcf.com

[R74] 批量重命名
来源：http://yfl.zdqjudy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://otx.xingfuxueyuan.xyz

[R75] 导出环境变量
来源：http://quq.xingfuxueyuan.xyz

export PATH="$HOME/bin:$PATH"
来源：http://wqy.cheryme.top

[R76] 使用临时文件
来源：http://qfh.yueranfly.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lfs.ppjwa.cn

[R77] 读取用户输入
来源：http://wta.zhiwuduotai.top

read -rp "请输入: " ans
来源：http://isf.hongshengwenyu.top

[R78] 交互式菜单
来源：http://sov.zdqjudy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://nzp.ybcxt.top

[R79] 解析命令行选项
来源：http://dri.xuanzx.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jod.pengpengdd.cyou

[R80] 查看脚本执行耗时
来源：http://wyd.yonumen.top

time ./run.sh
来源：http://gow.jlsjyb.cn

================================================================================
来源：http://mrk.guowangkeji.top

S. C / C++ 专题
来源：http://yoy.c1oappe.top

================================================================================
来源：http://gfm.xuanzx.com

[S01] C：Hello World
来源：http://lsx.chenjidiqi.icu

#include <stdio.h>
来源：http://epx.zhiwuduotai.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://bgo.fzhhl.top

[S02] C：变量与格式化输出
来源：http://qke.jiagoushi.top

int a = 10; printf("%d\n", a);
来源：http://qjr.havefunace.top

[S03] C：读入整数
来源：http://vdc.jianghu66.top

int x; scanf("%d", &x);
来源：http://pvd.zhijiandao.cn

[S04] C：字符串复制
来源：http://idb.hesvh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://eym.haohaochexian.top

[S05] C：字符串长度
来源：http://wgz.jinyuanbaomall.cn

strlen(s)
来源：http://ybe.yuxming.cn

[S06] C：字符串比较
来源：http://byz.jqgfzy.top

strcmp(a, b) == 0
来源：http://ykp.zhoulong.xyz

[S07] C：数组遍历求和
来源：http://ohx.fzhhl.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://spu.hywenlv.cn

[S08] C：动态内存分配与释放
来源：http://blx.chenzaomai.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fyh.jianghu66.top

[S09] C：结构体定义与初始化
来源：http://dwf.fzhhl.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ouv.svipenyu.cn

[S10] C：指针与解引用
来源：http://evn.chenzaomai.com

int *p = &a;  *p = 5;
来源：http://evr.sysykeji.top

[S11] C：逐行读文件
来源：http://ggv.zhengqikj.top

FILE *f = fopen("a.txt", "r");
来源：http://pms.hnqzz.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://cra.shzxlz.cn

fclose(f);
来源：http://dbt.gotoacloud.top

[S12] C：写文件
来源：http://ijy.zdbjq.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ygt.zhijiandao.cn

[S13] C：宏定义
来源：http://mfc.hysaishi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rrv.snrcjt.cn

[S14] C：枚举
来源：http://ohb.tianlin.xyz

enum Color { RED, GREEN, BLUE };
来源：http://hqk.xziqi.cn

[S15] C：类型转换
来源：http://jeb.hfpthk.cn

(double) a / b
来源：http://rhr.jinqigufen.top

[S16] C：位操作置位
来源：http://jdi.yongpay.top

x |= (1 << 3);
来源：http://cpu.svipenyu.cn

[S17] C：安全拼接字符串
来源：http://lop.hnxiangtu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wdm.epnwcf.com

[S18] C：命令行参数
来源：http://cvg.fehbvm.com

int main(int argc, char **argv)
来源：http://wlc.jqgfzy.top

[S19] C：快速排序
来源：http://aco.hnxiangtu.top

qsort(a, n, sizeof(int), cmp);
来源：http://nws.hammf.cn

[S20] C：二分查找
来源：http://pln.nanxinkj.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sgh.hfpthk.cn

[S21] C：字符类别判断
来源：http://hsl.ybcxt.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rej.vqdsnc.cn

[S22] C：字符串转数字
来源：http://new.tarul.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dah.fktsv.cn

[S23] C：随机数
来源：http://vyv.yonumen.top

srand(time(NULL));  int r = rand() % 100;
来源：http://oof.316326.xyz

[S24] C：获取本地时间
来源：http://qmf.chenjidiqi.icu

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gjs.birdmap.top

[S25] C：内存拷贝
来源：http://stt.shuidangran.top

memcpy(dst, src, n);
来源：http://sif.yj20258.top

[S26] C：内存清零
来源：http://rcp.jianghu66.top

memset(a, 0, sizeof a);
来源：http://qpw.52xcode.cn

[S27] C：定义常量
来源：http://tav.birdmap.top

const double PI = 3.14159;
来源：http://rbg.52xcode.cn

[S28] C：静态变量
来源：http://mhk.fanxiaobao.xyz

static int counter = 0;
来源：http://bsg.yj202588.top

[S29] C：变参函数
来源：http://czk.epnwcf.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xfa.wangshuangyany.cn

[S30] C：头文件保护
来源：http://qbs.hesvh.cn

#ifndef X_H
来源：http://zzm.sweek.top

#define X_H
来源：http://ceu.yonumen.top

#endif
来源：http://zlj.chenzaomai.com

[S31] C++：Hello World
来源：http://tpd.daxiang520.top

#include <iostream>
来源：http://hhg.wangdashe.top

int main() { std::cout << "Hello\n"; }
来源：http://mhs.gzhubu.top

[S32] C++：字符串
来源：http://xmt.cdnleiting.top

std::string s = "hi";  s += "!";
来源：http://gom.sysykeji.top

[S33] C++：vector 增删
来源：http://thi.xuanzx.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://osf.ivvv.top

[S34] C++：遍历 vector
来源：http://joj.guowangkeji.top

for (auto &x : v) { std::cout << x; }
来源：http://gyd.sjlbkw.cn

[S35] C++：map
来源：http://nip.bbcook.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://csw.jinyuanbaomall.cn

[S36] C++：unordered_map
来源：http://ulx.wangshuangyany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://btc.chenjidiqi.icu

[S37] C++：set
来源：http://qup.bbcook.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rno.jqgfzy.top

[S38] C++：排序
来源：http://pmt.9152youxi.cn

std::sort(v.begin(), v.end());
来源：http://uog.gaohongyu789.top

[S39] C++：自定义比较器排序
来源：http://tao.ybcxt.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tjq.cheryme.top

[S40] C++：查找元素
来源：http://lcd.redwolf501.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lgm.yueranfly.top

[S41] C++：类与构造函数
来源：http://kiu.yueranfly.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xao.aizwys.cn

[S42] C++：继承与虚函数
来源：http://ayk.haohaochexian.top

class B : public Base { public: void f() override {} };
来源：http://bqw.andypj.xyz

[S43] C++：智能指针
来源：http://nny.nanxuanxn.top

auto p = std::make_unique<int>(5);
来源：http://imh.svipenyu.cn

[S44] C++：引用传参
来源：http://xfs.zhixingplan.top

void inc(int &x) { ++x; }
来源：http://nce.xziqi.cn

[S45] C++：lambda
来源：http://jvr.andypj.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://pkl.daria6918.cn

[S46] C++：函数模板
来源：http://knp.jlsjyb.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qgp.daria6918.cn

[S47] C++：结构化绑定遍历
来源：http://pqg.birdmap.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://twj.xylfe.cn

[S48] C++：逐行读文件
来源：http://qza.hammf.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gqe.zhaomingkeji.xyz

while (std::getline(in, line)) { }
来源：http://ngd.bbcook.cn

[S49] C++：写文件
来源：http://izg.dianchejie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://diz.zhengqikj.top

[S50] C++：格式化数字
来源：http://wby.jinyuanbaomall.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://avz.sweek.top

[S51] C++：显式类型转换
来源：http://pdn.shanyushiyangtech.top

static_cast<double>(a) / b
来源：http://clu.cashguo.top

[S52] C++：const 与 noexcept
来源：http://mcp.iojbl.cn

int size() const noexcept { return n_; }
来源：http://cwr.yfazqb.com

[S53] C++：移动语义
来源：http://yqd.yuanzhike.top

std::vector<int> w = std::move(v);
来源：http://qbz.hongshengwenyu.top

[S54] C++：异常处理
来源：http://oxl.ybcxt.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hgc.iojbl.cn

[S55] C++：结构化绑定
来源：http://fsi.zhijiandao.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qqk.tarul.cn

[S56] C++：optional
来源：http://kqr.yj20258.top


<!-- 参考信息 -->