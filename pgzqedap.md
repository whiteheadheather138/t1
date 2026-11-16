代发 wailian999

[Q84] 去除首尾空格
来源：http://kyu.hammf.cn

SELECT TRIM(name) FROM users;
来源：http://qse.cashguo.top

[Q85] 数值取整
来源：http://nae.wangshuangyany.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zer.tarul.cn

[Q86] 读取 JSON 字段
来源：http://tuq.ydjk.org.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://agb.tanke756.top

[Q87] JSON 字段做条件
来源：http://mhq.jianghu66.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vzl.birdmap.top

[Q88] 行转列（条件聚合）
来源：http://fmi.xziqi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nju.hcnkem.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://obs.cqqwz.cn

[Q89] 判断表是否存在
来源：http://kzo.chenlongwang.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sug.fehbvm.com

[Q90] 生成序号列
来源：http://vue.zhoulong.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hfi.smart0.xyz

================================================================================
来源：http://edx.shangyingyoupin.top

R. Bash 专题
来源：http://dfc.9152youxi.cn

================================================================================
来源：http://fps.shuidangran.top

[R01] shebang 与严格模式
来源：http://ddj.daria6918.cn

#!/usr/bin/env bash
来源：http://uih.havefunace.top

set -euo pipefail
来源：http://mvk.ivvv.top

[R02] 变量赋值与使用
来源：http://pvt.zhoulong.xyz

name="Tom"; echo "$name"
来源：http://jdd.zhijiandao.cn

[R03] 只读变量
来源：http://tqx.zdqjudy.top

readonly PI=3.14
来源：http://cst.yanxiufei.cn

[R04] 位置参数
来源：http://gpc.gogol.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ujn.zhijiandao.cn

[R05] 参数默认值
来源：http://lxs.ppjwa.cn

name="${1:-default}"
来源：http://yxz.hfpthk.cn

[R06] 判断命令是否存在
来源：http://ehj.hfpthk.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://okj.guannengcc.top

[R07] if 判断文件
来源：http://vst.zycfv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ghj.epnwcf.com

[R08] 数值比较
来源：http://iun.ydzc1.top

if (( a > b )); then echo "a 更大"; fi
来源：http://odg.zhoulong.xyz

[R09] 字符串比较
来源：http://isz.hongshengwenyu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://axz.ydzc1.top

[R10] 正则匹配
来源：http://zoh.jlsjyb.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ulw.hywenlv.cn

[R11] case 多分支
来源：http://ymg.pengpengdd.cyou

case "$1" in
来源：http://xse.dashuyun.cn

start) echo "启动" ;;
来源：http://cst.jinqigufen.top

stop)  echo "停止" ;;
来源：http://uyj.mhx1999.top

*)     echo "未知命令" ;;
来源：http://udb.cheryme.top

esac
来源：http://nlw.ybcxt.top

[R12] for 遍历文件
来源：http://ejd.tianlin.xyz

for f in *.txt; do echo "$f"; done
来源：http://kgu.jlsjyb.cn

[R13] for 计数循环
来源：http://gcx.havefunace.top

for i in {1..10}; do echo "$i"; done
来源：http://plf.andypj.xyz

[R14] C 风格 for
来源：http://zkk.xylfe.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://emm.kuanghao11.cn

[R15] while 逐行读文件
来源：http://xuk.daria6918.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dow.ybcxt.top

[R16] until 等待条件
来源：http://ivu.tianlin.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zdx.tarul.cn

[R17] 数组定义与取值
来源：http://xes.meibo888.top

arr=(a b c); echo "${arr[0]}"
来源：http://erj.yuanzhike.top

[R18] 遍历数组
来源：http://egz.snrcjt.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vmh.fktsv.cn

[R19] 数组长度
来源：http://gaa.xuanzx.com

echo "${#arr[@]}"
来源：http://frh.yvedp.cn

[R20] 关联数组（字典）
来源：http://hcx.redwolf501.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xgp.pengpengdd.cyou

[R21] 字符串长度
来源：http://ude.yvedp.cn

echo "${#s}"
来源：http://nay.pycfn.com

[R22] 截取子串
来源：http://qsx.hysaishi.cn

echo "${s:0:5}"
来源：http://gjz.sweek.top

[R23] 字符串替换
来源：http://shj.jinqigufen.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wne.hammf.cn

[R24] 大小写转换
来源：http://yme.xuanzx.com

echo "${s^^}"; echo "${s,,}"
来源：http://iqc.epnwcf.com

[R25] 去后缀 / 去前缀
来源：http://uql.ppjwa.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://chf.shanyushiyangtech.top

[R26] 命令替换
来源：http://kdd.redwolf501.top

now=$(date +%F); echo "$now"
来源：http://nps.gzhubu.top

[R27] 算术展开
来源：http://lii.chenjidiqi.icu

echo $((1 + 2 * 3))
来源：http://dss.nanxinkj.top

[R28] 浮点运算
来源：http://dcr.feifeiyinyue.top

echo "scale=2; 10/3" | bc
来源：http://jne.uphjek.com

[R29] 定义函数
来源：http://hvo.pycfn.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xnj.chenlongwang.top

[R30] 函数返回状态码
来源：http://xqa.yueranfly.top

f() { return 0; }; f || echo "失败了"
来源：http://lnk.birdmap.top

[R31] 局部变量
来源：http://ymz.jyoumei.cn

f() { local x=1; echo "$x"; }
来源：http://kfr.9152youxi.cn

[R32] 参数个数校验
来源：http://bae.yueranfly.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hqs.feifeiyinyue.top

[R33] 捕获错误并提示行号
来源：http://kpe.tian-w.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fks.dashuyun.cn

[R34] 退出时清理
来源：http://jqm.cdnleiting.top

trap 'rm -f "$tmp"' EXIT
来源：http://zfs.ydzc1.top

[R35] 后台执行并等待
来源：http://ubn.jinghuilouyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qnv.ydzc1.top

[R36] 并发执行多个任务
来源：http://rtd.aizwys.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uyu.dianchejie.cn

[R37] 把输出赋给变量
来源：http://tqx.shanyushiyangtech.top

files=$(ls -1)
来源：http://ewa.ppjwa.cn

[R38] 管道串联
来源：http://kjx.shuidangran.top

cat a.txt | grep -i error | wc -l
来源：http://jub.ydzc1.top

[R39] 重定向标准输出与错误
来源：http://ksc.birdmap.top

cmd > out.log 2>&1
来源：http://dpi.iojbl.cn

[R40] 追加写日志
来源：http://ajs.ydjk.org.cn

echo "log" >> out.log
来源：http://csh.hammf.cn

[R41] 丢弃输出
来源：http://gpz.tianlin.xyz

cmd >/dev/null 2>&1
来源：http://ugd.birdmap.top

[R42] 输入重定向
来源：http://ozz.hnxiangtu.top

wc -l < a.txt
来源：http://qsy.cheryme.top

[R43] 按名字查找文件
来源：http://hiz.andypj.xyz

find . -name "*.log" -type f
来源：http://rmy.daria6918.cn

[R44] 按修改时间查找
来源：http://xls.cashguo.top

find . -mtime -7 -type f
来源：http://zbt.chenlongwang.top

[R45] 批量删除
来源：http://gcb.yueranfly.top

find . -name "*.tmp" -delete
来源：http://ikm.shanyushiyangtech.top

[R46] 递归替换文件内容
来源：http://eyz.daxiang520.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mxl.gzhubu.top

[R47] sed 单行替换
来源：http://wvr.xinyue.icu

sed -i 's/foo/bar/g' a.txt
来源：http://vro.gogol.net.cn

[R48] awk 取指定列
来源：http://vyk.sysykeji.top

awk '{print $1, $3}' a.txt
来源：http://lwj.meibo888.top

[R49] awk 带条件
来源：http://biq.hcnkem.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fcf.hesvh.cn

[R50] awk 求和
来源：http://ple.yangfankeji.com

awk '{s += $2} END {print s}' a.txt
来源：http://wuk.hnqzz.top

[R51] 排序去重取前几
来源：http://etc.sysykeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://sub.zhixingplan.top

[R52] 统计行数
来源：http://yer.quarkkingdee.top

wc -l a.txt
来源：http://ccm.cashguo.top

[R53] 查看文件头与实时尾
来源：http://epv.gzhubu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mqj.cdnleiting.top

[R54] 比较两个文件
来源：http://dip.jinghuilouyu.cn

diff a.txt b.txt
来源：http://chx.uphjek.com

[R55] 压缩与解压
来源：http://ufm.yuxming.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ulg.tanke756.top

[R56] 远程拷贝
来源：http://wln.yueranfly.top

scp file user@host:/path/
来源：http://sgx.ivvv.top

[R57] 远程执行命令
来源：http://gtx.gaohongyu789.top

ssh user@host 'uptime'
来源：http://exd.cucudq.cn

[R58] 下载文件
来源：http://ksj.nwbrower.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cwb.yangfankeji.com

[R59] 发 POST JSON
来源：http://orw.yj20258.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://emx.yueranfly.top

[R60] 只看 HTTP 状态码
来源：http://nnn.yueranfly.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dwj.jqgfzy.top

[R61] 磁盘占用
来源：http://ucz.ivvv.top

df -h;  du -sh *
来源：http://jxw.vehdjk.com

[R62] 找最占空间的文件
来源：http://isu.sxryk.cn

du -ah . | sort -rh | head -10
来源：http://miq.hysaishi.cn

[R63] 内存与进程
来源：http://fby.sweek.top

free -h;  ps aux | grep nginx
来源：http://mhh.shuidangran.top

[R64] 结束进程
来源：http://lzi.yuanzhike.top

kill -9 $(pgrep -f app.py)
来源：http://zgs.sysykeji.top

[R65] 查看端口占用
来源：http://ecl.sxryk.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ecb.ivvv.top

[R66] 定时任务
来源：http://qqe.iojbl.cn

crontab -e;  crontab -l
来源：http://ssx.redwolf501.top

[R67] 生成随机十六进制串
来源：http://gwa.hammf.cn

openssl rand -hex 16
来源：http://esg.shanyushiyangtech.top

[R68] 计算文件校验值
来源：http://pda.yongpay.top

sha256sum a.txt;  md5sum a.txt
来源：http://crb.andypj.xyz

[R69] 生成随机密码
来源：http://lic.jiagoushi.top

head -c 16 /dev/urandom | base64
来源：http://imd.smart0.xyz

[R70] 时间戳与互转
来源：http://bvh.bjfxy.top

date +%s;  date -d @1700000000
来源：http://mmv.ppjwa.cn

[R71] 日期格式化
来源：http://scn.jinqigufen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qqf.bjfxy.top

[R72] 等待端口就绪
来源：http://kkp.zhijiandao.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://clw.ydjk.org.cn

[R73] 分割大日志
来源：http://fdw.xylfe.cn

split -l 1000 big.log part_
来源：http://ouz.zhixingplan.top

[R74] 批量重命名
来源：http://qjz.kuanghao11.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rmj.yangfankeji.com

[R75] 导出环境变量
来源：http://huf.ydjk.org.cn

export PATH="$HOME/bin:$PATH"
来源：http://aii.chenzaomai.com

[R76] 使用临时文件
来源：http://epe.yongpay.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://run.ywan-chungtsiang.top

[R77] 读取用户输入
来源：http://jqc.yangfankeji.com

read -rp "请输入: " ans
来源：http://uku.pycfn.com

[R78] 交互式菜单
来源：http://btr.sjlbkw.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ovf.jianghu66.top

[R79] 解析命令行选项
来源：http://pdz.yj20258888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bwn.9152youxi.cn

[R80] 查看脚本执行耗时
来源：http://dwd.shanyushiyangtech.top

time ./run.sh
来源：http://mgy.sufxvd.cn

================================================================================
来源：http://rny.cqqwz.cn

S. C / C++ 专题
来源：http://dth.yuanzhike.top

================================================================================
来源：http://oqp.havefunace.top

[S01] C：Hello World
来源：http://pvz.jinyuanbaomall.cn

#include <stdio.h>
来源：http://mpw.zhijiandao.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cnb.hfpthk.cn

[S02] C：变量与格式化输出
来源：http://dxb.yvedp.cn

int a = 10; printf("%d\n", a);
来源：http://cfw.jinqigufen.top

[S03] C：读入整数
来源：http://niv.cashguo.top

int x; scanf("%d", &x);
来源：http://crj.hysaishi.cn

[S04] C：字符串复制
来源：http://ata.jqgfzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://hwc.ivvv.top

[S05] C：字符串长度
来源：http://sap.daxiang520.top

strlen(s)
来源：http://xhq.tarul.cn

[S06] C：字符串比较
来源：http://oed.hammf.cn

strcmp(a, b) == 0
来源：http://evu.feifeiyinyue.top

[S07] C：数组遍历求和
来源：http://qns.zhongyouzk.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hxz.svipenyu.cn

[S08] C：动态内存分配与释放
来源：http://egw.yj20258.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hvd.zhongyouzk.top

[S09] C：结构体定义与初始化
来源：http://hjx.xingfuxueyuan.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oib.quarkkingdee.top

[S10] C：指针与解引用
来源：http://mco.dashuyun.cn

int *p = &a;  *p = 5;
来源：http://cff.pycfn.com

[S11] C：逐行读文件
来源：http://rbh.mhx1999.top

FILE *f = fopen("a.txt", "r");
来源：http://okq.tanke756.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://aik.xuanzx.com

fclose(f);
来源：http://egv.fktsv.cn

[S12] C：写文件
来源：http://tfq.ydzc1.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rgg.sweek.top

[S13] C：宏定义
来源：http://euf.redwolf501.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tfh.hfpthk.cn

[S14] C：枚举
来源：http://trj.shanyushiyangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://lki.hywenlv.cn

[S15] C：类型转换
来源：http://kjx.guannengcc.top

(double) a / b
来源：http://snm.ybcxt.top

[S16] C：位操作置位
来源：http://mwj.yj20258.top

x |= (1 << 3);
来源：http://eof.zhijiandao.cn

[S17] C：安全拼接字符串
来源：http://cze.zdbjq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hrl.nanxuanxn.top

[S18] C：命令行参数
来源：http://swx.meibo888.top

int main(int argc, char **argv)
来源：http://ijf.vqdsnc.cn

[S19] C：快速排序
来源：http://qdm.daxiang520.top

qsort(a, n, sizeof(int), cmp);
来源：http://tcs.zdqjudy.top

[S20] C：二分查找
来源：http://ktp.zdqjudy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://prl.tian-w.cn

[S21] C：字符类别判断
来源：http://dpo.kuanghao11.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cmr.gzhubu.top

[S22] C：字符串转数字
来源：http://jyo.jiagoushi.top

atoi("42");  strtod("3.14", NULL);
来源：http://pcd.xinyue.icu

[S23] C：随机数
来源：http://aii.shangyingyoupin.top

srand(time(NULL));  int r = rand() % 100;
来源：http://twq.zhoulong.xyz

[S24] C：获取本地时间
来源：http://ggl.shzxlz.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ruu.fzhhl.top

[S25] C：内存拷贝
来源：http://rdp.ybcxt.top

memcpy(dst, src, n);
来源：http://knm.fktsv.cn

[S26] C：内存清零
来源：http://jiw.vqdsnc.cn

memset(a, 0, sizeof a);
来源：http://plj.nanxuanxn.top

[S27] C：定义常量
来源：http://ljm.fanxiaobao.xyz

const double PI = 3.14159;
来源：http://bzn.jqgfzy.top

[S28] C：静态变量
来源：http://qlj.uphjek.com

static int counter = 0;
来源：http://eia.cdnleiting.top

[S29] C：变参函数
来源：http://dah.shzxlz.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qbd.tianlin.xyz

[S30] C：头文件保护
来源：http://pgt.hnxiangtu.top

#ifndef X_H
来源：http://xob.daxiang520.top

#define X_H
来源：http://dif.jlsjyb.cn

#endif
来源：http://nfm.zycfv.cn

[S31] C++：Hello World
来源：http://mgj.zycfv.cn

#include <iostream>
来源：http://tya.jinghuilouyu.cn

int main() { std::cout << "Hello\n"; }
来源：http://ucq.xziqi.cn

[S32] C++：字符串
来源：http://kbp.yj202588.top

std::string s = "hi";  s += "!";
来源：http://fhc.birdmap.top

[S33] C++：vector 增删
来源：http://hla.fehbvm.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bkh.haohaochexian.top

[S34] C++：遍历 vector
来源：http://lgd.daria6918.cn

for (auto &x : v) { std::cout << x; }
来源：http://esz.ywan-chungtsiang.top

[S35] C++：map
来源：http://wxr.svipenyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jsu.smart0.xyz

[S36] C++：unordered_map
来源：http://vxt.yueranfly.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hdo.9152youxi.cn

[S37] C++：set
来源：http://ubw.fanxiaobao.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://izc.cucudq.cn

[S38] C++：排序
来源：http://ziz.redwolf501.top

std::sort(v.begin(), v.end());
来源：http://gup.yueranfly.top

[S39] C++：自定义比较器排序
来源：http://yjc.zycfv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ozp.yongpay.top

[S40] C++：查找元素
来源：http://ump.tianlin.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gei.sysykeji.top

[S41] C++：类与构造函数
来源：http://qce.hongshengwenyu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jgw.pycfn.com

[S42] C++：继承与虚函数
来源：http://vlm.hysaishi.cn

class B : public Base { public: void f() override {} };
来源：http://bqf.guannengcc.top

[S43] C++：智能指针
来源：http://hfs.yj20258.top

auto p = std::make_unique<int>(5);
来源：http://kav.yanxiufei.cn

[S44] C++：引用传参
来源：http://nuc.zycfv.cn

void inc(int &x) { ++x; }
来源：http://xlh.yj202588.top

[S45] C++：lambda
来源：http://lxc.sxryk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pzq.zycfv.cn

[S46] C++：函数模板
来源：http://zak.hongshengwenyu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jdo.tian-w.cn

[S47] C++：结构化绑定遍历
来源：http://nub.c1oappe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vmj.pycfn.com

[S48] C++：逐行读文件
来源：http://byb.hongshengwenyu.top

std::ifstream in("a.txt");  std::string line;
来源：http://ija.chenzaomai.com

while (std::getline(in, line)) { }
来源：http://oia.nanxuanxn.top

[S49] C++：写文件
来源：http://rnz.hfpthk.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mmx.chenlongwang.top

[S50] C++：格式化数字
来源：http://hzz.hesvh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tdf.gotoacloud.top

[S51] C++：显式类型转换
来源：http://pio.gaohongyu789.top

static_cast<double>(a) / b
来源：http://eeo.xziqi.cn

[S52] C++：const 与 noexcept
来源：http://vdv.shanyushiyangkeji.top

int size() const noexcept { return n_; }
来源：http://pto.daxiang520.top

[S53] C++：移动语义
来源：http://sck.yj202588.top

std::vector<int> w = std::move(v);
来源：http://aif.yongpay.top

[S54] C++：异常处理
来源：http://rig.jinyuanbaomall.cn


<!-- 参考信息 -->