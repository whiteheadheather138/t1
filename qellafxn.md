代发 wailian999

[Q82] 字符长度与字节长度
来源：http://mhi.tarul.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bhx.shanyushiyangtech.top

[Q83] 大小写转换
来源：http://pky.cucudq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://atb.chenjidiqi.icu

[Q84] 去除首尾空格
来源：http://nkp.guowangkeji.top

SELECT TRIM(name) FROM users;
来源：http://uiu.vehdjk.com

[Q85] 数值取整
来源：http://pkq.yj20258888.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pep.ppjwa.cn

[Q86] 读取 JSON 字段
来源：http://rks.haohaochexian.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://stb.tian-w.cn

[Q87] JSON 字段做条件
来源：http://bqq.zhijiandao.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vhe.xylfe.cn

[Q88] 行转列（条件聚合）
来源：http://vtc.yj202588.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jaf.tarul.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vzy.shzxlz.cn

[Q89] 判断表是否存在
来源：http://hdu.jinghuilouyu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uvh.wangdashe.top

[Q90] 生成序号列
来源：http://tzj.ydjk.org.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jtl.shanyushiyangtech.top

================================================================================
来源：http://gpi.meibo888.top

R. Bash 专题
来源：http://uxe.shuidangran.top

================================================================================
来源：http://mis.zhixingplan.top

[R01] shebang 与严格模式
来源：http://ztb.gaohongyu789.top

#!/usr/bin/env bash
来源：http://qtz.feifeiyinyue.top

set -euo pipefail
来源：http://xgk.aizwys.cn

[R02] 变量赋值与使用
来源：http://mtl.zhaomingkeji.xyz

name="Tom"; echo "$name"
来源：http://tiw.sysykeji.top

[R03] 只读变量
来源：http://nvr.hywenlv.cn

readonly PI=3.14
来源：http://kao.sxryk.cn

[R04] 位置参数
来源：http://hdq.mhx1999.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://igt.shanyushiyangkeji.top

[R05] 参数默认值
来源：http://tja.sweek.top

name="${1:-default}"
来源：http://wkh.yuxming.cn

[R06] 判断命令是否存在
来源：http://eem.jinqigufen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://juq.gogol.net.cn

[R07] if 判断文件
来源：http://pke.0kj1m.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mbs.52xcode.cn

[R08] 数值比较
来源：http://yyf.wangshuangyany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ezm.pycfn.com

[R09] 字符串比较
来源：http://mla.yueranfly.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dwj.zhongyouzk.top

[R10] 正则匹配
来源：http://pcb.ctjpmb.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://btf.epnwcf.com

[R11] case 多分支
来源：http://dhm.nanxuanxn.top

case "$1" in
来源：http://djk.wangdashe.top

start) echo "启动" ;;
来源：http://ujz.zycfv.cn

stop)  echo "停止" ;;
来源：http://oih.wangshuangyany.cn

*)     echo "未知命令" ;;
来源：http://omu.aizwys.cn

esac
来源：http://gmp.ehwqpu.com

[R12] for 遍历文件
来源：http://tvs.hysaishi.cn

for f in *.txt; do echo "$f"; done
来源：http://pmq.vqdsnc.cn

[R13] for 计数循环
来源：http://cdm.0kj1m.cn

for i in {1..10}; do echo "$i"; done
来源：http://nsk.yueranfly.top

[R14] C 风格 for
来源：http://mhi.daxiang520.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qnz.ydjk.org.cn

[R15] while 逐行读文件
来源：http://pwa.vqdsnc.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vyt.316326.xyz

[R16] until 等待条件
来源：http://jri.xinyue.icu

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wtw.bbcook.cn

[R17] 数组定义与取值
来源：http://xet.jinqigfzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://lfu.hongshengwenyu.top

[R18] 遍历数组
来源：http://aoz.gzhubu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rob.shanyushiyangtech.top

[R19] 数组长度
来源：http://bkg.zhengqikj.top

echo "${#arr[@]}"
来源：http://lfv.gogol.net.cn

[R20] 关联数组（字典）
来源：http://ugl.ybcxt.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://srh.chenlongwang.top

[R21] 字符串长度
来源：http://fve.shangyingyoupin.top

echo "${#s}"
来源：http://xpe.gaohongyu789.top

[R22] 截取子串
来源：http://svv.52xcode.cn

echo "${s:0:5}"
来源：http://cze.ctjpmb.com

[R23] 字符串替换
来源：http://qbw.52xcode.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yct.aizwys.cn

[R24] 大小写转换
来源：http://gpm.jiagoushi.top

echo "${s^^}"; echo "${s,,}"
来源：http://qnq.yj20258888.top

[R25] 去后缀 / 去前缀
来源：http://mqe.tianlin.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://qta.hammf.cn

[R26] 命令替换
来源：http://iyl.jyoumei.cn

now=$(date +%F); echo "$now"
来源：http://onj.cdnleiting.top

[R27] 算术展开
来源：http://doj.jinqigfzy.top

echo $((1 + 2 * 3))
来源：http://hij.jiagoushi.top

[R28] 浮点运算
来源：http://oia.jiagoushi.top

echo "scale=2; 10/3" | bc
来源：http://twp.ybcxt.top

[R29] 定义函数
来源：http://eiq.cucudq.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pas.chenjidiqi.icu

[R30] 函数返回状态码
来源：http://iac.ctjpmb.com

f() { return 0; }; f || echo "失败了"
来源：http://hnu.hfpthk.cn

[R31] 局部变量
来源：http://jqv.yanxiufei.cn

f() { local x=1; echo "$x"; }
来源：http://ugb.daria6918.cn

[R32] 参数个数校验
来源：http://uqj.tianlin.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lff.haohaochexian.top

[R33] 捕获错误并提示行号
来源：http://dsq.cheryme.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xzb.jinqigufen.top

[R34] 退出时清理
来源：http://flc.zhoulong.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://swi.hysaishi.cn

[R35] 后台执行并等待
来源：http://eqy.hysaishi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://djo.xziqi.cn

[R36] 并发执行多个任务
来源：http://khf.yuxming.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qjf.ppjwa.cn

[R37] 把输出赋给变量
来源：http://bgf.zhixingplan.top

files=$(ls -1)
来源：http://zmr.xingfuxueyuan.xyz

[R38] 管道串联
来源：http://rkz.bjfxy.top

cat a.txt | grep -i error | wc -l
来源：http://slh.yanxiufei.cn

[R39] 重定向标准输出与错误
来源：http://pfm.ybcxt.top

cmd > out.log 2>&1
来源：http://gki.vehdjk.com

[R40] 追加写日志
来源：http://ltr.ivvv.top

echo "log" >> out.log
来源：http://pml.smart0.xyz

[R41] 丢弃输出
来源：http://kqn.c1oappe.top

cmd >/dev/null 2>&1
来源：http://mkc.zhixingplan.top

[R42] 输入重定向
来源：http://flw.zhengqikj.top

wc -l < a.txt
来源：http://jbs.shuidangran.top

[R43] 按名字查找文件
来源：http://bow.shangyingyoupin.top

find . -name "*.log" -type f
来源：http://mym.shanyushiyangtech.top

[R44] 按修改时间查找
来源：http://mwz.sweek.top

find . -mtime -7 -type f
来源：http://okv.ppjwa.cn

[R45] 批量删除
来源：http://iis.ydzc1.top

find . -name "*.tmp" -delete
来源：http://gnu.havefunace.top

[R46] 递归替换文件内容
来源：http://llv.zhijiandao.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ppz.ctjpmb.com

[R47] sed 单行替换
来源：http://ygo.jinqigufen.top

sed -i 's/foo/bar/g' a.txt
来源：http://epj.pycfn.com

[R48] awk 取指定列
来源：http://rrr.zhengqikj.top

awk '{print $1, $3}' a.txt
来源：http://qqk.shangyingyoupin.top

[R49] awk 带条件
来源：http://iow.shuidangran.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yxa.shzxlz.cn

[R50] awk 求和
来源：http://pzb.xinyue.icu

awk '{s += $2} END {print s}' a.txt
来源：http://zsb.cdnleiting.top

[R51] 排序去重取前几
来源：http://bgw.vehdjk.com

sort a.txt | uniq -c | sort -rn | head
来源：http://olm.ehwqpu.com

[R52] 统计行数
来源：http://hka.zhijiandao.cn

wc -l a.txt
来源：http://udd.hammf.cn

[R53] 查看文件头与实时尾
来源：http://ixs.ydjk.org.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qjm.wangdashe.top

[R54] 比较两个文件
来源：http://ric.ehwqpu.com

diff a.txt b.txt
来源：http://awy.shanyushiyangkeji.top

[R55] 压缩与解压
来源：http://sla.ehwqpu.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cmn.ppjwa.cn

[R56] 远程拷贝
来源：http://uto.jinqigufen.top

scp file user@host:/path/
来源：http://bii.0kj1m.cn

[R57] 远程执行命令
来源：http://ofu.dashuyun.cn

ssh user@host 'uptime'
来源：http://pvj.fanxiaobao.xyz

[R58] 下载文件
来源：http://ooe.wangdashe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tjo.nanxinkj.top

[R59] 发 POST JSON
来源：http://scn.aibaodan.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://spi.guowangkeji.top

[R60] 只看 HTTP 状态码
来源：http://xzm.fehbvm.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://chg.birdmap.top

[R61] 磁盘占用
来源：http://zao.gaohongyu789.top

df -h;  du -sh *
来源：http://chq.svipenyu.cn

[R62] 找最占空间的文件
来源：http://fjz.birdmap.top

du -ah . | sort -rh | head -10
来源：http://utg.yanxiufei.cn

[R63] 内存与进程
来源：http://nkd.mhx1999.top

free -h;  ps aux | grep nginx
来源：http://jiu.shzxlz.cn

[R64] 结束进程
来源：http://gix.dianchejie.cn

kill -9 $(pgrep -f app.py)
来源：http://gdr.sufxvd.cn

[R65] 查看端口占用
来源：http://dgi.0kj1m.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://epg.yueranfly.top

[R66] 定时任务
来源：http://bqh.gaohongyu789.top

crontab -e;  crontab -l
来源：http://yzz.cashguo.top

[R67] 生成随机十六进制串
来源：http://phc.nanxuanxn.top

openssl rand -hex 16
来源：http://fya.daria6918.cn

[R68] 计算文件校验值
来源：http://bav.gogol.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://oij.jqgfzy.top

[R69] 生成随机密码
来源：http://stp.tarul.cn

head -c 16 /dev/urandom | base64
来源：http://azu.gaohongyu789.top

[R70] 时间戳与互转
来源：http://brn.zhiwuduotai.top

date +%s;  date -d @1700000000
来源：http://hyp.shuidangran.top

[R71] 日期格式化
来源：http://hrh.sxryk.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nwe.pycfn.com

[R72] 等待端口就绪
来源：http://czg.cucudq.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://eom.ydjk.org.cn

[R73] 分割大日志
来源：http://siw.jqgufenzy.top

split -l 1000 big.log part_
来源：http://jif.yanxiufei.cn

[R74] 批量重命名
来源：http://dri.yvedp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dlt.zdbjq.cn

[R75] 导出环境变量
来源：http://vzw.jinqigfzy.top

export PATH="$HOME/bin:$PATH"
来源：http://gxn.jianghu66.top

[R76] 使用临时文件
来源：http://lmy.andypj.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mjw.zhixingplan.top

[R77] 读取用户输入
来源：http://uxu.sjlbkw.cn

read -rp "请输入: " ans
来源：http://qtw.aizwys.cn

[R78] 交互式菜单
来源：http://ibf.kuanghao11.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fsm.zhixingplan.top

[R79] 解析命令行选项
来源：http://ovt.tarul.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://szc.bjfxy.top

[R80] 查看脚本执行耗时
来源：http://xlo.yongpay.top

time ./run.sh
来源：http://gyc.zhongyouzk.top

================================================================================
来源：http://fgg.yj20258.top

S. C / C++ 专题
来源：http://xcj.shuidangran.top

================================================================================
来源：http://ktx.sysykeji.top

[S01] C：Hello World
来源：http://qbb.yj202588.top

#include <stdio.h>
来源：http://jvd.zhixingplan.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://mma.epnwcf.com

[S02] C：变量与格式化输出
来源：http://luo.tianlin.xyz

int a = 10; printf("%d\n", a);
来源：http://weg.zhaomingkeji.xyz

[S03] C：读入整数
来源：http://efk.yj20258888.top

int x; scanf("%d", &x);
来源：http://mbi.shzxlz.cn

[S04] C：字符串复制
来源：http://gcm.hesvh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fet.zdbjq.cn

[S05] C：字符串长度
来源：http://nsx.316326.xyz

strlen(s)
来源：http://fnl.hfpthk.cn

[S06] C：字符串比较
来源：http://cut.316326.xyz

strcmp(a, b) == 0
来源：http://bpe.yuxming.cn

[S07] C：数组遍历求和
来源：http://tgh.ehwqpu.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bhg.bbcook.cn

[S08] C：动态内存分配与释放
来源：http://zuq.jqgufenzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ewu.shzxlz.cn

[S09] C：结构体定义与初始化
来源：http://urg.zycfv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vzj.zdqjudy.top

[S10] C：指针与解引用
来源：http://smz.ehwqpu.com

int *p = &a;  *p = 5;
来源：http://dhr.jinyuanbaomall.cn

[S11] C：逐行读文件
来源：http://eab.wangshuangyany.cn

FILE *f = fopen("a.txt", "r");
来源：http://zzh.cashguo.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://tyh.jinghuilouyu.cn

fclose(f);
来源：http://xxt.shzxlz.cn

[S12] C：写文件
来源：http://utp.jinqigufen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ire.guannengcc.top

[S13] C：宏定义
来源：http://teh.tianlin.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ksg.yanxiufei.cn

[S14] C：枚举
来源：http://myq.bjfxy.top

enum Color { RED, GREEN, BLUE };
来源：http://cuc.ybcxt.top

[S15] C：类型转换
来源：http://gsr.cdnleiting.top

(double) a / b
来源：http://mfx.gaohongyu789.top

[S16] C：位操作置位
来源：http://jwd.nwbrower.top

x |= (1 << 3);
来源：http://jxr.aibaodan.cn

[S17] C：安全拼接字符串
来源：http://zpg.haohaochexian.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cyb.yonumen.top

[S18] C：命令行参数
来源：http://rwf.sufxvd.cn

int main(int argc, char **argv)
来源：http://khn.jianghu66.top

[S19] C：快速排序
来源：http://qfv.tian-w.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xvb.sxryk.cn

[S20] C：二分查找
来源：http://ckd.ctjpmb.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kkk.9152youxi.cn

[S21] C：字符类别判断
来源：http://stz.yuxming.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://aal.shanyushiyangtech.top

[S22] C：字符串转数字
来源：http://rqj.jinyuanbaomall.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rqx.iojbl.cn

[S23] C：随机数
来源：http://qcr.nanxuanxn.top

srand(time(NULL));  int r = rand() % 100;
来源：http://alo.ydzc1.top

[S24] C：获取本地时间
来源：http://vyk.jlsjyb.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pgb.bbcook.cn

[S25] C：内存拷贝
来源：http://ahs.316326.xyz

memcpy(dst, src, n);
来源：http://rkf.zhongyouzk.top

[S26] C：内存清零
来源：http://asi.jinqigfzy.top

memset(a, 0, sizeof a);
来源：http://qvx.yvedp.cn

[S27] C：定义常量
来源：http://qxl.quarkkingdee.top

const double PI = 3.14159;
来源：http://hnt.yanxiufei.cn

[S28] C：静态变量
来源：http://rgw.yuanzhike.top

static int counter = 0;
来源：http://ljd.hongshengwenyu.top

[S29] C：变参函数
来源：http://unr.smart0.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qml.chenjidiqi.icu

[S30] C：头文件保护
来源：http://fkm.yj20258888.top

#ifndef X_H
来源：http://gcy.feifeiyinyue.top

#define X_H
来源：http://afx.zycfv.cn

#endif
来源：http://eka.sjlbkw.cn

[S31] C++：Hello World
来源：http://pzy.nanxuanxn.top

#include <iostream>
来源：http://eqr.cashguo.top

int main() { std::cout << "Hello\n"; }
来源：http://tcr.shangyingyoupin.top

[S32] C++：字符串
来源：http://chg.tianlin.xyz

std::string s = "hi";  s += "!";
来源：http://ddj.yj202588.top

[S33] C++：vector 增删
来源：http://taj.hnxiangtu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tzd.dashuyun.cn

[S34] C++：遍历 vector
来源：http://dzc.wangshuangyany.cn

for (auto &x : v) { std::cout << x; }
来源：http://soj.fktsv.cn

[S35] C++：map
来源：http://reb.jqgfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gpz.zdbjq.cn

[S36] C++：unordered_map
来源：http://ibu.cdnleiting.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qlw.ywan-chungtsiang.top

[S37] C++：set
来源：http://pcn.yuxming.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xav.52xcode.cn

[S38] C++：排序
来源：http://kps.xylfe.cn

std::sort(v.begin(), v.end());
来源：http://gef.xylfe.cn

[S39] C++：自定义比较器排序
来源：http://gjh.daria6918.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://htm.cashguo.top

[S40] C++：查找元素
来源：http://mls.yj202588.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cjr.jianghu66.top

[S41] C++：类与构造函数
来源：http://zmu.dashuyun.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cwx.tarul.cn

[S42] C++：继承与虚函数
来源：http://qup.cucudq.cn

class B : public Base { public: void f() override {} };
来源：http://zvt.redwolf501.top

[S43] C++：智能指针
来源：http://qzz.guowangkeji.top

auto p = std::make_unique<int>(5);
来源：http://yqv.sysykeji.top

[S44] C++：引用传参
来源：http://mcd.snrcjt.cn

void inc(int &x) { ++x; }
来源：http://rcm.chenlongwang.top

[S45] C++：lambda
来源：http://ohb.hnqzz.top

auto add = [](int a, int b) { return a + b; };
来源：http://tqi.zycfv.cn

[S46] C++：函数模板
来源：http://nth.zycfv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wtv.hcnkem.com

[S47] C++：结构化绑定遍历
来源：http://tpt.52xcode.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ufs.jiagoushi.top

[S48] C++：逐行读文件
来源：http://oxd.c1oappe.top

std::ifstream in("a.txt");  std::string line;
来源：http://kyv.shzxlz.cn

while (std::getline(in, line)) { }
来源：http://wxt.316326.xyz

[S49] C++：写文件
来源：http://sho.jinqigfzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gof.cucudq.cn

[S50] C++：格式化数字
来源：http://vrt.jinyuanbaomall.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ihx.birdmap.top

[S51] C++：显式类型转换
来源：http://dgt.daria6918.cn

static_cast<double>(a) / b
来源：http://ept.c1oappe.top

[S52] C++：const 与 noexcept
来源：http://lqm.jinqigfzy.top


<!-- 参考信息 -->