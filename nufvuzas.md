代发 wailian999

[Q86] 读取 JSON 字段
来源：http://ywq.jinqigufen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nke.jianghu66.top

[Q87] JSON 字段做条件
来源：http://ijf.hywenlv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gtr.ehwqpu.com

[Q88] 行转列（条件聚合）
来源：http://khm.tianlin.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sry.hongshengwenyu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uhl.yj202588.top

[Q89] 判断表是否存在
来源：http://dvk.zhixingplan.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ben.hesvh.cn

[Q90] 生成序号列
来源：http://xwd.mhx1999.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hsz.sysykeji.top

================================================================================
来源：http://qcx.vqdsnc.cn

R. Bash 专题
来源：http://ifc.c1oappe.top

================================================================================
来源：http://poy.aibaodan.cn

[R01] shebang 与严格模式
来源：http://hmd.chenjidiqi.icu

#!/usr/bin/env bash
来源：http://xfb.yfazqb.com

set -euo pipefail
来源：http://xwi.daria6918.cn

[R02] 变量赋值与使用
来源：http://hiz.dashuyun.cn

name="Tom"; echo "$name"
来源：http://aie.tianlin.xyz

[R03] 只读变量
来源：http://ech.xuetiantiany.cn

readonly PI=3.14
来源：http://xsz.ydjk.org.cn

[R04] 位置参数
来源：http://esl.meibo888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://iyi.yanxiufei.cn

[R05] 参数默认值
来源：http://nni.iojbl.cn

name="${1:-default}"
来源：http://bpm.hfpthk.cn

[R06] 判断命令是否存在
来源：http://abg.hnqzz.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gbl.tarul.cn

[R07] if 判断文件
来源：http://nsn.ehwqpu.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://szc.gogol.net.cn

[R08] 数值比较
来源：http://yvs.andypj.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://dsq.jlsjyb.cn

[R09] 字符串比较
来源：http://uxj.yfazqb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hyu.shangyingyoupin.top

[R10] 正则匹配
来源：http://aqv.dashuyun.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ksa.tanke756.top

[R11] case 多分支
来源：http://lli.fehbvm.com

case "$1" in
来源：http://htc.yuxming.cn

start) echo "启动" ;;
来源：http://yqj.redwolf501.top

stop)  echo "停止" ;;
来源：http://idh.zdqjudy.top

*)     echo "未知命令" ;;
来源：http://mcv.zhijiandao.cn

esac
来源：http://tup.jiagoushi.top

[R12] for 遍历文件
来源：http://mhl.xuetiantiany.cn

for f in *.txt; do echo "$f"; done
来源：http://dfb.daria6918.cn

[R13] for 计数循环
来源：http://kjt.jqgufenzy.top

for i in {1..10}; do echo "$i"; done
来源：http://yqx.sjlbkw.cn

[R14] C 风格 for
来源：http://raw.zdbjq.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qbg.haohaochexian.top

[R15] while 逐行读文件
来源：http://kal.bbcook.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dfj.shanyushiyangkeji.top

[R16] until 等待条件
来源：http://kii.zhaomingkeji.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blf.hfpthk.cn

[R17] 数组定义与取值
来源：http://nmb.hnxiangtu.top

arr=(a b c); echo "${arr[0]}"
来源：http://tee.fktsv.cn

[R18] 遍历数组
来源：http://qdn.jiagoushi.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kvp.yonumen.top

[R19] 数组长度
来源：http://vjq.yangfankeji.com

echo "${#arr[@]}"
来源：http://egv.vehdjk.com

[R20] 关联数组（字典）
来源：http://aci.yangfankeji.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rdv.xylfe.cn

[R21] 字符串长度
来源：http://twx.hnxiangtu.top

echo "${#s}"
来源：http://wai.aizwys.cn

[R22] 截取子串
来源：http://tvk.mhx1999.top

echo "${s:0:5}"
来源：http://eev.zhongyouzk.top

[R23] 字符串替换
来源：http://mco.fengsongda.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://guk.ctjpmb.com

[R24] 大小写转换
来源：http://ujn.chenlongwang.top

echo "${s^^}"; echo "${s,,}"
来源：http://lnv.cqqwz.cn

[R25] 去后缀 / 去前缀
来源：http://kvs.hnxiangtu.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://iif.jyoumei.cn

[R26] 命令替换
来源：http://xvv.fehbvm.com

now=$(date +%F); echo "$now"
来源：http://nfr.birdmap.top

[R27] 算术展开
来源：http://tbw.aibaodan.cn

echo $((1 + 2 * 3))
来源：http://dyb.ybcxt.top

[R28] 浮点运算
来源：http://swj.shuidangran.top

echo "scale=2; 10/3" | bc
来源：http://nea.zhijiandao.cn

[R29] 定义函数
来源：http://vpa.nanxinkj.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hxt.snrcjt.cn

[R30] 函数返回状态码
来源：http://hpl.birdmap.top

f() { return 0; }; f || echo "失败了"
来源：http://emv.snrcjt.cn

[R31] 局部变量
来源：http://ujw.dashuyun.cn

f() { local x=1; echo "$x"; }
来源：http://cnf.shzxlz.cn

[R32] 参数个数校验
来源：http://hqa.dashuyun.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ebs.yanxiufei.cn

[R33] 捕获错误并提示行号
来源：http://ple.yueranfly.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wgx.yongpay.top

[R34] 退出时清理
来源：http://dtm.hcnkem.com

trap 'rm -f "$tmp"' EXIT
来源：http://idw.fzhhl.top

[R35] 后台执行并等待
来源：http://iuk.52xcode.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qae.yj20258.top

[R36] 并发执行多个任务
来源：http://zom.jlsjyb.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://iap.hnxiangtu.top

[R37] 把输出赋给变量
来源：http://orf.chenjidiqi.icu

files=$(ls -1)
来源：http://kkg.zdqjudy.top

[R38] 管道串联
来源：http://wsp.kuanghao11.cn

cat a.txt | grep -i error | wc -l
来源：http://hqk.tanke756.top

[R39] 重定向标准输出与错误
来源：http://uvq.gotoacloud.top

cmd > out.log 2>&1
来源：http://oig.zycfv.cn

[R40] 追加写日志
来源：http://hoi.smart0.xyz

echo "log" >> out.log
来源：http://jln.sweek.top

[R41] 丢弃输出
来源：http://bhl.ppjwa.cn

cmd >/dev/null 2>&1
来源：http://lwp.sxryk.cn

[R42] 输入重定向
来源：http://xoe.zhoulong.xyz

wc -l < a.txt
来源：http://tkh.jiagoushi.top

[R43] 按名字查找文件
来源：http://ijt.mhx1999.top

find . -name "*.log" -type f
来源：http://omg.0kj1m.cn

[R44] 按修改时间查找
来源：http://urd.jianghu66.top

find . -mtime -7 -type f
来源：http://zac.zhongyouzk.top

[R45] 批量删除
来源：http://rjp.kuanghao11.cn

find . -name "*.tmp" -delete
来源：http://umf.cdnleiting.top

[R46] 递归替换文件内容
来源：http://eat.ydjk.org.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wmw.ydjk.org.cn

[R47] sed 单行替换
来源：http://gxp.pycfn.com

sed -i 's/foo/bar/g' a.txt
来源：http://wjp.yongpay.top

[R48] awk 取指定列
来源：http://kak.jianghu66.top

awk '{print $1, $3}' a.txt
来源：http://ysq.zhaomingkeji.xyz

[R49] awk 带条件
来源：http://oik.vqdsnc.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bwv.mhx1999.top

[R50] awk 求和
来源：http://ilt.jianghu66.top

awk '{s += $2} END {print s}' a.txt
来源：http://rxl.hnxiangtu.top

[R51] 排序去重取前几
来源：http://llt.gogol.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vvk.dashuyun.cn

[R52] 统计行数
来源：http://iuc.52xcode.cn

wc -l a.txt
来源：http://tjw.hcnkem.com

[R53] 查看文件头与实时尾
来源：http://tbn.ybcxt.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fxf.jiagoushi.top

[R54] 比较两个文件
来源：http://jca.fzhhl.top

diff a.txt b.txt
来源：http://tqr.hcnkem.com

[R55] 压缩与解压
来源：http://bon.sysykeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dnb.sxryk.cn

[R56] 远程拷贝
来源：http://ehy.chenjidiqi.icu

scp file user@host:/path/
来源：http://moy.daria6918.cn

[R57] 远程执行命令
来源：http://axz.shanyushiyangkeji.top

ssh user@host 'uptime'
来源：http://yqj.ivvv.top

[R58] 下载文件
来源：http://pgm.cheryme.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dqq.gaohongyu789.top

[R59] 发 POST JSON
来源：http://dhi.dashuyun.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dsm.sweek.top

[R60] 只看 HTTP 状态码
来源：http://eob.hcnkem.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cso.zhixingplan.top

[R61] 磁盘占用
来源：http://ban.epnwcf.com

df -h;  du -sh *
来源：http://mmw.yongpay.top

[R62] 找最占空间的文件
来源：http://ovx.xingfuxueyuan.xyz

du -ah . | sort -rh | head -10
来源：http://txu.zhiwuduotai.top

[R63] 内存与进程
来源：http://bjr.jinyuanbaomall.cn

free -h;  ps aux | grep nginx
来源：http://wbw.yj20258888.top

[R64] 结束进程
来源：http://hoc.xingfuxueyuan.xyz

kill -9 $(pgrep -f app.py)
来源：http://fyd.fktsv.cn

[R65] 查看端口占用
来源：http://dgr.xylfe.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://leo.xziqi.cn

[R66] 定时任务
来源：http://kdo.jlsjyb.cn

crontab -e;  crontab -l
来源：http://twq.tanke756.top

[R67] 生成随机十六进制串
来源：http://mmc.316326.xyz

openssl rand -hex 16
来源：http://gbe.cqqwz.cn

[R68] 计算文件校验值
来源：http://wji.pengpengdd.cyou

sha256sum a.txt;  md5sum a.txt
来源：http://fdd.hongshengwenyu.top

[R69] 生成随机密码
来源：http://twa.xingfuxueyuan.xyz

head -c 16 /dev/urandom | base64
来源：http://fxf.hammf.cn

[R70] 时间戳与互转
来源：http://xhf.gaohongyu789.top

date +%s;  date -d @1700000000
来源：http://gta.aizwys.cn

[R71] 日期格式化
来源：http://uzi.zhoulong.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://yiw.andypj.xyz

[R72] 等待端口就绪
来源：http://aim.jqgfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://irg.cqqwz.cn

[R73] 分割大日志
来源：http://sgl.bbcook.cn

split -l 1000 big.log part_
来源：http://eda.zdqjudy.top

[R74] 批量重命名
来源：http://lsa.xuanzx.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://naj.daxiang520.top

[R75] 导出环境变量
来源：http://ksh.jinyuanbaomall.cn

export PATH="$HOME/bin:$PATH"
来源：http://pzu.tianlin.xyz

[R76] 使用临时文件
来源：http://rke.shangyingyoupin.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rcd.cqqwz.cn

[R77] 读取用户输入
来源：http://cbt.yj20258.top

read -rp "请输入: " ans
来源：http://jta.ydzc1.top

[R78] 交互式菜单
来源：http://iox.0kj1m.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dli.tanke756.top

[R79] 解析命令行选项
来源：http://jar.bbcook.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jzx.cheryme.top

[R80] 查看脚本执行耗时
来源：http://vfc.fanxiaobao.xyz

time ./run.sh
来源：http://reh.shzxlz.cn

================================================================================
来源：http://mdq.zhongyouzk.top

S. C / C++ 专题
来源：http://kyn.jyoumei.cn

================================================================================
来源：http://xmc.ydzc1.top

[S01] C：Hello World
来源：http://ihp.ydjk.org.cn

#include <stdio.h>
来源：http://lux.ybcxt.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://djq.haohaochexian.top

[S02] C：变量与格式化输出
来源：http://ixj.9152youxi.cn

int a = 10; printf("%d\n", a);
来源：http://iuo.ybcxt.top

[S03] C：读入整数
来源：http://qqr.nwbrower.top

int x; scanf("%d", &x);
来源：http://uto.svipenyu.cn

[S04] C：字符串复制
来源：http://vcb.nanxuanxn.top

char dst[32]; strcpy(dst, "hi");
来源：http://glx.sysykeji.top

[S05] C：字符串长度
来源：http://uqs.fengsongda.top

strlen(s)
来源：http://fup.52xcode.cn

[S06] C：字符串比较
来源：http://ssl.ppjwa.cn

strcmp(a, b) == 0
来源：http://llp.gzhubu.top

[S07] C：数组遍历求和
来源：http://yiq.wangshuangyany.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ftf.jinghuilouyu.cn

[S08] C：动态内存分配与释放
来源：http://jmu.bjfxy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ebx.zdqjudy.top

[S09] C：结构体定义与初始化
来源：http://cwh.dianchejie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vqv.sjlbkw.cn

[S10] C：指针与解引用
来源：http://sar.pengpengdd.cyou

int *p = &a;  *p = 5;
来源：http://lqr.tianlin.xyz

[S11] C：逐行读文件
来源：http://xmu.hywenlv.cn

FILE *f = fopen("a.txt", "r");
来源：http://ayz.hfpthk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://soi.hammf.cn

fclose(f);
来源：http://vpk.hysaishi.cn

[S12] C：写文件
来源：http://hez.hfpthk.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kbp.shangyingyoupin.top

[S13] C：宏定义
来源：http://aot.jianghu66.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fwi.hnqzz.top

[S14] C：枚举
来源：http://kcx.haohaochexian.top

enum Color { RED, GREEN, BLUE };
来源：http://xkz.zhixingplan.top

[S15] C：类型转换
来源：http://fgq.wangdashe.top

(double) a / b
来源：http://hrv.andypj.xyz

[S16] C：位操作置位
来源：http://mcn.yuxming.cn

x |= (1 << 3);
来源：http://okh.zdbjq.cn

[S17] C：安全拼接字符串
来源：http://str.316326.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ptk.sjlbkw.cn

[S18] C：命令行参数
来源：http://bum.jinqigfzy.top

int main(int argc, char **argv)
来源：http://kqj.pycfn.com

[S19] C：快速排序
来源：http://tzi.yuxming.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qng.shanyushiyangkeji.top

[S20] C：二分查找
来源：http://epe.hongshengwenyu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://glu.zhijiandao.cn

[S21] C：字符类别判断
来源：http://hpp.guowangkeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tkc.yuxming.cn

[S22] C：字符串转数字
来源：http://uui.jinghuilouyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gur.jianghu66.top

[S23] C：随机数
来源：http://dop.gotoacloud.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ucq.guowangkeji.top

[S24] C：获取本地时间
来源：http://xsz.yueranfly.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jkg.vehdjk.com

[S25] C：内存拷贝
来源：http://evp.meibo888.top

memcpy(dst, src, n);
来源：http://lsh.chenlongwang.top

[S26] C：内存清零
来源：http://jyc.daxiang520.top

memset(a, 0, sizeof a);
来源：http://hsu.aibaodan.cn

[S27] C：定义常量
来源：http://pet.chenzaomai.com

const double PI = 3.14159;
来源：http://cvs.fanxiaobao.xyz

[S28] C：静态变量
来源：http://qks.yuxming.cn

static int counter = 0;
来源：http://faz.snrcjt.cn

[S29] C：变参函数
来源：http://lhb.redwolf501.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xik.pycfn.com

[S30] C：头文件保护
来源：http://ztj.fzhhl.top

#ifndef X_H
来源：http://kom.chenjidiqi.icu

#define X_H
来源：http://rnf.jlsjyb.cn

#endif
来源：http://ieh.smart0.xyz

[S31] C++：Hello World
来源：http://tpd.chenjidiqi.icu

#include <iostream>
来源：http://xju.gaohongyu789.top

int main() { std::cout << "Hello\n"; }
来源：http://syn.xuanzx.com

[S32] C++：字符串
来源：http://noq.ydzc1.top

std::string s = "hi";  s += "!";
来源：http://hzv.ppjwa.cn

[S33] C++：vector 增删
来源：http://aek.hongshengwenyu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uxk.ehwqpu.com

[S34] C++：遍历 vector
来源：http://clj.vehdjk.com

for (auto &x : v) { std::cout << x; }
来源：http://jwh.hfpthk.cn

[S35] C++：map
来源：http://yda.shangyingyoupin.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eaa.ctjpmb.com

[S36] C++：unordered_map
来源：http://aae.jinqigufen.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zch.cqqwz.cn

[S37] C++：set
来源：http://jyc.yj202588.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uwm.jlsjyb.cn

[S38] C++：排序
来源：http://lpj.meibo888.top

std::sort(v.begin(), v.end());
来源：http://qbw.c1oappe.top

[S39] C++：自定义比较器排序
来源：http://zqy.sufxvd.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://txw.sysykeji.top

[S40] C++：查找元素
来源：http://txw.tian-w.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cee.daria6918.cn

[S41] C++：类与构造函数
来源：http://eyk.sysykeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hym.ctjpmb.com

[S42] C++：继承与虚函数
来源：http://via.zhixingplan.top

class B : public Base { public: void f() override {} };
来源：http://kou.andypj.xyz

[S43] C++：智能指针
来源：http://ldk.epnwcf.com

auto p = std::make_unique<int>(5);
来源：http://avx.c1oappe.top

[S44] C++：引用传参
来源：http://wmw.shanyushiyangkeji.top

void inc(int &x) { ++x; }
来源：http://fru.dashuyun.cn

[S45] C++：lambda
来源：http://bod.jiagoushi.top

auto add = [](int a, int b) { return a + b; };
来源：http://osk.zhaomingkeji.xyz

[S46] C++：函数模板
来源：http://sqc.xziqi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tei.xingfuxueyuan.xyz

[S47] C++：结构化绑定遍历
来源：http://gsq.snrcjt.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tgx.ywan-chungtsiang.top

[S48] C++：逐行读文件
来源：http://ual.havefunace.top

std::ifstream in("a.txt");  std::string line;
来源：http://fne.hcnkem.com

while (std::getline(in, line)) { }
来源：http://lcy.sysykeji.top

[S49] C++：写文件
来源：http://spi.c1oappe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sfy.9152youxi.cn

[S50] C++：格式化数字
来源：http://gvh.zhaomingkeji.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mgw.xingfuxueyuan.xyz

[S51] C++：显式类型转换
来源：http://klr.daxiang520.top

static_cast<double>(a) / b
来源：http://wwx.xziqi.cn

[S52] C++：const 与 noexcept
来源：http://uvn.sjlbkw.cn

int size() const noexcept { return n_; }
来源：http://vir.hfpthk.cn

[S53] C++：移动语义
来源：http://sxw.zhengqikj.top

std::vector<int> w = std::move(v);
来源：http://oqh.andypj.xyz

[S54] C++：异常处理
来源：http://ngb.jinghuilouyu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kbp.cashguo.top

[S55] C++：结构化绑定
来源：http://reb.fengsongda.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lvb.fzhhl.top

[S56] C++：optional
来源：http://ogs.ctjpmb.com


<!-- 参考信息 -->