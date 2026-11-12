代发 wailian999

[Q86] 读取 JSON 字段
来源：http://jxt.sjlbkw.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://trv.wangshuangyany.cn

[Q87] JSON 字段做条件
来源：http://lop.ydzc1.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://urv.hesvh.cn

[Q88] 行转列（条件聚合）
来源：http://ihb.hnqzz.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xnc.cheryme.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dlt.0kj1m.cn

[Q89] 判断表是否存在
来源：http://fle.hywenlv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nge.uphjek.com

[Q90] 生成序号列
来源：http://bau.aizwys.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cgt.zhijiandao.cn

================================================================================
来源：http://ufe.yongpay.top

R. Bash 专题
来源：http://ijf.jiagoushi.top

================================================================================
来源：http://aox.shuidangran.top

[R01] shebang 与严格模式
来源：http://nkw.jqgufenzy.top

#!/usr/bin/env bash
来源：http://qji.ydzc1.top

set -euo pipefail
来源：http://xhx.52xcode.cn

[R02] 变量赋值与使用
来源：http://hoq.nanxuanxn.top

name="Tom"; echo "$name"
来源：http://xmv.zycfv.cn

[R03] 只读变量
来源：http://zci.uphjek.com

readonly PI=3.14
来源：http://olu.guowangkeji.top

[R04] 位置参数
来源：http://rqo.cashguo.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://irp.yongpay.top

[R05] 参数默认值
来源：http://iah.jiagoushi.top

name="${1:-default}"
来源：http://xlo.jinqigfzy.top

[R06] 判断命令是否存在
来源：http://szt.hfpthk.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rzz.feifeiyinyue.top

[R07] if 判断文件
来源：http://qbc.xuanzx.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ans.guannengcc.top

[R08] 数值比较
来源：http://sji.ywan-chungtsiang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://dzl.mhx1999.top

[R09] 字符串比较
来源：http://vtq.yanxiufei.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vyb.jlsjyb.cn

[R10] 正则匹配
来源：http://tyo.cashguo.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xca.nanxinkj.top

[R11] case 多分支
来源：http://qpe.jinyuanbaomall.cn

case "$1" in
来源：http://fmz.zhiwuduotai.top

start) echo "启动" ;;
来源：http://bwq.nanxinkj.top

stop)  echo "停止" ;;
来源：http://njw.zhaomingkeji.xyz

*)     echo "未知命令" ;;
来源：http://omn.fktsv.cn

esac
来源：http://bpb.hysaishi.cn

[R12] for 遍历文件
来源：http://wrs.shanyushiyangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://kwu.fanxiaobao.xyz

[R13] for 计数循环
来源：http://nyc.smart0.xyz

for i in {1..10}; do echo "$i"; done
来源：http://iat.aizwys.cn

[R14] C 风格 for
来源：http://pin.andypj.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dkf.zhongyouzk.top

[R15] while 逐行读文件
来源：http://jed.hnqzz.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://suy.aibaodan.cn

[R16] until 等待条件
来源：http://pkj.redwolf501.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fsy.redwolf501.top

[R17] 数组定义与取值
来源：http://umj.yj20258888.top

arr=(a b c); echo "${arr[0]}"
来源：http://rhe.vehdjk.com

[R18] 遍历数组
来源：http://irg.yj202588.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://irz.xylfe.cn

[R19] 数组长度
来源：http://hjr.0kj1m.cn

echo "${#arr[@]}"
来源：http://xjd.fzhhl.top

[R20] 关联数组（字典）
来源：http://exp.birdmap.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qag.zhiwuduotai.top

[R21] 字符串长度
来源：http://tgn.meibo888.top

echo "${#s}"
来源：http://pum.zhiwuduotai.top

[R22] 截取子串
来源：http://rrk.wangdashe.top

echo "${s:0:5}"
来源：http://tzf.zhiwuduotai.top

[R23] 字符串替换
来源：http://cly.zdbjq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://elh.xuanzx.com

[R24] 大小写转换
来源：http://sxt.svipenyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://omr.zhixingplan.top

[R25] 去后缀 / 去前缀
来源：http://ray.bbcook.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qfr.quarkkingdee.top

[R26] 命令替换
来源：http://tyx.dashuyun.cn

now=$(date +%F); echo "$now"
来源：http://zhj.gotoacloud.top

[R27] 算术展开
来源：http://gnc.zhixingplan.top

echo $((1 + 2 * 3))
来源：http://mly.xziqi.cn

[R28] 浮点运算
来源：http://kgo.hongshengwenyu.top

echo "scale=2; 10/3" | bc
来源：http://fog.feifeiyinyue.top

[R29] 定义函数
来源：http://ela.uphjek.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mrs.hnqzz.top

[R30] 函数返回状态码
来源：http://tpe.sweek.top

f() { return 0; }; f || echo "失败了"
来源：http://oin.yangfankeji.com

[R31] 局部变量
来源：http://qdi.chenjidiqi.icu

f() { local x=1; echo "$x"; }
来源：http://ypk.shuidangran.top

[R32] 参数个数校验
来源：http://iih.guannengcc.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qoa.chenlongwang.top

[R33] 捕获错误并提示行号
来源：http://xty.bbcook.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lrg.yj20258.top

[R34] 退出时清理
来源：http://rlj.yangfankeji.com

trap 'rm -f "$tmp"' EXIT
来源：http://xbk.xuanzx.com

[R35] 后台执行并等待
来源：http://hjr.chenjidiqi.icu

sleep 5 & pid=$!; wait "$pid"
来源：http://dir.aizwys.cn

[R36] 并发执行多个任务
来源：http://pmc.cashguo.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://elv.fzhhl.top

[R37] 把输出赋给变量
来源：http://rqa.tianlin.xyz

files=$(ls -1)
来源：http://obp.ppjwa.cn

[R38] 管道串联
来源：http://uxm.jinqigfzy.top

cat a.txt | grep -i error | wc -l
来源：http://wlc.shuidangran.top

[R39] 重定向标准输出与错误
来源：http://hth.yuxming.cn

cmd > out.log 2>&1
来源：http://uqw.jqgfzy.top

[R40] 追加写日志
来源：http://zcx.shuidangran.top

echo "log" >> out.log
来源：http://naj.zycfv.cn

[R41] 丢弃输出
来源：http://kqt.meibo888.top

cmd >/dev/null 2>&1
来源：http://xaz.cheryme.top

[R42] 输入重定向
来源：http://faj.nanxuanxn.top

wc -l < a.txt
来源：http://rqm.aizwys.cn

[R43] 按名字查找文件
来源：http://cgo.jiagoushi.top

find . -name "*.log" -type f
来源：http://kzg.haohaochexian.top

[R44] 按修改时间查找
来源：http://xhr.gotoacloud.top

find . -mtime -7 -type f
来源：http://qkp.tianlin.xyz

[R45] 批量删除
来源：http://stx.yanxiufei.cn

find . -name "*.tmp" -delete
来源：http://udu.epnwcf.com

[R46] 递归替换文件内容
来源：http://lfl.hnqzz.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nii.jqgfzy.top

[R47] sed 单行替换
来源：http://wnr.jinghuilouyu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xvr.epnwcf.com

[R48] awk 取指定列
来源：http://phw.jinqigufen.top

awk '{print $1, $3}' a.txt
来源：http://ptw.yj20258888.top

[R49] awk 带条件
来源：http://mzu.sysykeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oor.zhaomingkeji.xyz

[R50] awk 求和
来源：http://jbj.zdqjudy.top

awk '{s += $2} END {print s}' a.txt
来源：http://ttm.hcnkem.com

[R51] 排序去重取前几
来源：http://uiq.mhx1999.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ngc.sufxvd.cn

[R52] 统计行数
来源：http://lxd.havefunace.top

wc -l a.txt
来源：http://ikn.haohaochexian.top

[R53] 查看文件头与实时尾
来源：http://hgr.yj20258.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kww.andypj.xyz

[R54] 比较两个文件
来源：http://ayn.yuanzhike.top

diff a.txt b.txt
来源：http://wad.sysykeji.top

[R55] 压缩与解压
来源：http://ypz.xingfuxueyuan.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vdu.hysaishi.cn

[R56] 远程拷贝
来源：http://rbx.fehbvm.com

scp file user@host:/path/
来源：http://jjf.hcnkem.com

[R57] 远程执行命令
来源：http://tkb.tianlin.xyz

ssh user@host 'uptime'
来源：http://rbf.zdqjudy.top

[R58] 下载文件
来源：http://vbu.yj202588.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ktb.ivvv.top

[R59] 发 POST JSON
来源：http://lmx.52xcode.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jyb.zhoulong.xyz

[R60] 只看 HTTP 状态码
来源：http://gcp.yj202588.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zpf.sysykeji.top

[R61] 磁盘占用
来源：http://xdi.jinyuanbaomall.cn

df -h;  du -sh *
来源：http://amd.c1oappe.top

[R62] 找最占空间的文件
来源：http://ojf.hammf.cn

du -ah . | sort -rh | head -10
来源：http://pbh.birdmap.top

[R63] 内存与进程
来源：http://agz.iojbl.cn

free -h;  ps aux | grep nginx
来源：http://nxw.zhiwuduotai.top

[R64] 结束进程
来源：http://chc.chenlongwang.top

kill -9 $(pgrep -f app.py)
来源：http://yxi.fanxiaobao.xyz

[R65] 查看端口占用
来源：http://gqw.bjfxy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ayg.xziqi.cn

[R66] 定时任务
来源：http://bhx.mhx1999.top

crontab -e;  crontab -l
来源：http://vno.ehwqpu.com

[R67] 生成随机十六进制串
来源：http://trj.fktsv.cn

openssl rand -hex 16
来源：http://fno.yfazqb.com

[R68] 计算文件校验值
来源：http://bfm.chenjidiqi.icu

sha256sum a.txt;  md5sum a.txt
来源：http://rob.redwolf501.top

[R69] 生成随机密码
来源：http://jwo.zhiwuduotai.top

head -c 16 /dev/urandom | base64
来源：http://zwq.tian-w.cn

[R70] 时间戳与互转
来源：http://zmf.zhengqikj.top

date +%s;  date -d @1700000000
来源：http://zpc.pycfn.com

[R71] 日期格式化
来源：http://uhx.yongpay.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://nzj.ctjpmb.com

[R72] 等待端口就绪
来源：http://xlq.yuxming.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hky.epnwcf.com

[R73] 分割大日志
来源：http://pis.yuanzhike.top

split -l 1000 big.log part_
来源：http://ben.epnwcf.com

[R74] 批量重命名
来源：http://cpw.hywenlv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hea.cqqwz.cn

[R75] 导出环境变量
来源：http://dew.epnwcf.com

export PATH="$HOME/bin:$PATH"
来源：http://ivr.yangfankeji.com

[R76] 使用临时文件
来源：http://rog.fktsv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nui.mhx1999.top

[R77] 读取用户输入
来源：http://dnm.tanke756.top

read -rp "请输入: " ans
来源：http://lln.hysaishi.cn

[R78] 交互式菜单
来源：http://gqg.hammf.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cvu.ppjwa.cn

[R79] 解析命令行选项
来源：http://tvj.ydjk.org.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zur.yuxming.cn

[R80] 查看脚本执行耗时
来源：http://gqj.wangdashe.top

time ./run.sh
来源：http://odm.fanxiaobao.xyz

================================================================================
来源：http://feg.tarul.cn

S. C / C++ 专题
来源：http://lri.nwbrower.top

================================================================================
来源：http://yva.yangfankeji.com

[S01] C：Hello World
来源：http://cds.vqdsnc.cn

#include <stdio.h>
来源：http://xnc.mhx1999.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vpe.ywan-chungtsiang.top

[S02] C：变量与格式化输出
来源：http://gwn.ehwqpu.com

int a = 10; printf("%d\n", a);
来源：http://bmu.yvedp.cn

[S03] C：读入整数
来源：http://pnd.redwolf501.top

int x; scanf("%d", &x);
来源：http://xiv.jyoumei.cn

[S04] C：字符串复制
来源：http://klm.nanxuanxn.top

char dst[32]; strcpy(dst, "hi");
来源：http://zwh.316326.xyz

[S05] C：字符串长度
来源：http://kfu.smart0.xyz

strlen(s)
来源：http://ptb.316326.xyz

[S06] C：字符串比较
来源：http://ukh.aibaodan.cn

strcmp(a, b) == 0
来源：http://nvw.hongshengwenyu.top

[S07] C：数组遍历求和
来源：http://yoc.ppjwa.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gpd.smart0.xyz

[S08] C：动态内存分配与释放
来源：http://diu.tian-w.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wqk.yvedp.cn

[S09] C：结构体定义与初始化
来源：http://drm.yvedp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fmf.zhongyouzk.top

[S10] C：指针与解引用
来源：http://kjo.mhx1999.top

int *p = &a;  *p = 5;
来源：http://upw.zhixingplan.top

[S11] C：逐行读文件
来源：http://vpc.snrcjt.cn

FILE *f = fopen("a.txt", "r");
来源：http://scd.zdbjq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nct.epnwcf.com

fclose(f);
来源：http://fwz.yangfankeji.com

[S12] C：写文件
来源：http://rzf.redwolf501.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ubp.birdmap.top

[S13] C：宏定义
来源：http://bwy.aizwys.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ejn.xinyue.icu

[S14] C：枚举
来源：http://ryu.nanxuanxn.top

enum Color { RED, GREEN, BLUE };
来源：http://qlo.haohaochexian.top

[S15] C：类型转换
来源：http://usn.yueranfly.top

(double) a / b
来源：http://vde.zdqjudy.top

[S16] C：位操作置位
来源：http://siy.uphjek.com

x |= (1 << 3);
来源：http://dxz.jinqigufen.top

[S17] C：安全拼接字符串
来源：http://qcf.hysaishi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ger.52xcode.cn

[S18] C：命令行参数
来源：http://gjc.cashguo.top

int main(int argc, char **argv)
来源：http://enk.daxiang520.top

[S19] C：快速排序
来源：http://ynt.fehbvm.com

qsort(a, n, sizeof(int), cmp);
来源：http://ncf.fzhhl.top

[S20] C：二分查找
来源：http://rxk.yuanzhike.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eug.sufxvd.cn

[S21] C：字符类别判断
来源：http://uyx.nwbrower.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pcp.zhiwuduotai.top

[S22] C：字符串转数字
来源：http://wvg.hammf.cn

atoi("42");  strtod("3.14", NULL);
来源：http://smx.xziqi.cn

[S23] C：随机数
来源：http://nld.hongshengwenyu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://uwr.fktsv.cn

[S24] C：获取本地时间
来源：http://fma.shanyushiyangkeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://waz.sufxvd.cn

[S25] C：内存拷贝
来源：http://lpr.redwolf501.top

memcpy(dst, src, n);
来源：http://gyk.sjlbkw.cn

[S26] C：内存清零
来源：http://qxk.jinqigufen.top

memset(a, 0, sizeof a);
来源：http://vwq.kuanghao11.cn

[S27] C：定义常量
来源：http://uxd.yfazqb.com

const double PI = 3.14159;
来源：http://yuc.birdmap.top

[S28] C：静态变量
来源：http://pbe.bbcook.cn

static int counter = 0;
来源：http://ink.uphjek.com

[S29] C：变参函数
来源：http://uca.jqgufenzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qxy.shangyingyoupin.top

[S30] C：头文件保护
来源：http://pot.epnwcf.com

#ifndef X_H
来源：http://vpc.mhx1999.top

#define X_H
来源：http://dnv.ydzc1.top

#endif
来源：http://yyh.jinghuilouyu.cn

[S31] C++：Hello World
来源：http://xoi.pengpengdd.cyou

#include <iostream>
来源：http://eey.hnxiangtu.top

int main() { std::cout << "Hello\n"; }
来源：http://osx.zhengqikj.top

[S32] C++：字符串
来源：http://eqv.sweek.top

std::string s = "hi";  s += "!";
来源：http://ecz.sxryk.cn

[S33] C++：vector 增删
来源：http://kgy.shzxlz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bnf.nwbrower.top

[S34] C++：遍历 vector
来源：http://ksh.hongshengwenyu.top

for (auto &x : v) { std::cout << x; }
来源：http://gqe.redwolf501.top

[S35] C++：map
来源：http://uxc.jqgfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bvg.mhx1999.top

[S36] C++：unordered_map
来源：http://xax.yangfankeji.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rno.snrcjt.cn

[S37] C++：set
来源：http://umu.hnxiangtu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gbo.sufxvd.cn

[S38] C++：排序
来源：http://gsk.cucudq.cn

std::sort(v.begin(), v.end());
来源：http://rgx.shangyingyoupin.top

[S39] C++：自定义比较器排序
来源：http://wag.mhx1999.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://onm.bbcook.cn

[S40] C++：查找元素
来源：http://iwz.xingfuxueyuan.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cij.tanke756.top

[S41] C++：类与构造函数
来源：http://gxw.yj20258.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nol.hywenlv.cn

[S42] C++：继承与虚函数
来源：http://rja.ydjk.org.cn

class B : public Base { public: void f() override {} };
来源：http://ybc.cdnleiting.top

[S43] C++：智能指针
来源：http://whq.yangfankeji.com

auto p = std::make_unique<int>(5);
来源：http://sgx.cashguo.top

[S44] C++：引用传参
来源：http://xpg.cqqwz.cn

void inc(int &x) { ++x; }
来源：http://kzt.zhaomingkeji.xyz

[S45] C++：lambda
来源：http://hdn.jinyuanbaomall.cn

auto add = [](int a, int b) { return a + b; };
来源：http://byb.aizwys.cn

[S46] C++：函数模板
来源：http://nai.mhx1999.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://iyh.xuanzx.com

[S47] C++：结构化绑定遍历
来源：http://rlg.jinghuilouyu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dwn.guowangkeji.top

[S48] C++：逐行读文件
来源：http://hdo.wangshuangyany.cn

std::ifstream in("a.txt");  std::string line;
来源：http://iyl.yongpay.top

while (std::getline(in, line)) { }
来源：http://erl.tian-w.cn

[S49] C++：写文件
来源：http://agl.tian-w.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cbc.yuanzhike.top

[S50] C++：格式化数字
来源：http://ygx.shangyingyoupin.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://agi.gzhubu.top

[S51] C++：显式类型转换
来源：http://gqp.sjlbkw.cn

static_cast<double>(a) / b
来源：http://msp.aibaodan.cn

[S52] C++：const 与 noexcept
来源：http://crh.316326.xyz

int size() const noexcept { return n_; }
来源：http://oql.vqdsnc.cn

[S53] C++：移动语义
来源：http://xhd.jinghuilouyu.cn

std::vector<int> w = std::move(v);
来源：http://mjp.sufxvd.cn

[S54] C++：异常处理
来源：http://efv.jlsjyb.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dgj.wangshuangyany.cn

[S55] C++：结构化绑定
来源：http://edp.uphjek.com

auto [a, b] = std::make_pair(1, 2);
来源：http://oqh.quarkkingdee.top

[S56] C++：optional
来源：http://ghu.yfazqb.com


<!-- 参考信息 -->