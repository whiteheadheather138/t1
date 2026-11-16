代发 wailian999

[Q84] 去除首尾空格
来源：http://mxn.haohaochexian.top

SELECT TRIM(name) FROM users;
来源：http://oyx.zhaomingkeji.xyz

[Q85] 数值取整
来源：http://ino.hywenlv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qnr.snrcjt.cn

[Q86] 读取 JSON 字段
来源：http://nxa.yongpay.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gpx.sweek.top

[Q87] JSON 字段做条件
来源：http://fis.shangyingyoupin.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zxa.xylfe.cn

[Q88] 行转列（条件聚合）
来源：http://jkf.nanxuanxn.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sia.aizwys.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dsr.sxryk.cn

[Q89] 判断表是否存在
来源：http://wnf.meibo888.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://czb.shanyushiyangtech.top

[Q90] 生成序号列
来源：http://mbw.jyoumei.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jon.316326.xyz

================================================================================
来源：http://fjh.jianghu66.top

R. Bash 专题
来源：http://bri.jianghu66.top

================================================================================
来源：http://onk.yongpay.top

[R01] shebang 与严格模式
来源：http://kvp.316326.xyz

#!/usr/bin/env bash
来源：http://ibx.nwbrower.top

set -euo pipefail
来源：http://edu.mhx1999.top

[R02] 变量赋值与使用
来源：http://dpx.feifeiyinyue.top

name="Tom"; echo "$name"
来源：http://kjm.zycfv.cn

[R03] 只读变量
来源：http://iuq.gogol.net.cn

readonly PI=3.14
来源：http://mbb.yj20258888.top

[R04] 位置参数
来源：http://tfq.cdnleiting.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mzn.shzxlz.cn

[R05] 参数默认值
来源：http://kmf.fehbvm.com

name="${1:-default}"
来源：http://wbx.chenjidiqi.icu

[R06] 判断命令是否存在
来源：http://gak.yj202588.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vkw.zhixingplan.top

[R07] if 判断文件
来源：http://qnr.smart0.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yhi.guowangkeji.top

[R08] 数值比较
来源：http://ksz.cheryme.top

if (( a > b )); then echo "a 更大"; fi
来源：http://uuy.yuxming.cn

[R09] 字符串比较
来源：http://vlu.smart0.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gkv.fzhhl.top

[R10] 正则匹配
来源：http://blg.gzhubu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ite.yonumen.top

[R11] case 多分支
来源：http://ekk.xinyue.icu

case "$1" in
来源：http://ade.yvedp.cn

start) echo "启动" ;;
来源：http://kik.xingfuxueyuan.xyz

stop)  echo "停止" ;;
来源：http://zsf.meibo888.top

*)     echo "未知命令" ;;
来源：http://fko.ydzc1.top

esac
来源：http://gvo.tian-w.cn

[R12] for 遍历文件
来源：http://whf.fktsv.cn

for f in *.txt; do echo "$f"; done
来源：http://rbk.tarul.cn

[R13] for 计数循环
来源：http://aus.yj20258.top

for i in {1..10}; do echo "$i"; done
来源：http://vew.yvedp.cn

[R14] C 风格 for
来源：http://uzx.sweek.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uqr.jinqigfzy.top

[R15] while 逐行读文件
来源：http://seq.yueranfly.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://trr.ctjpmb.com

[R16] until 等待条件
来源：http://mvc.jqgfzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ndy.epnwcf.com

[R17] 数组定义与取值
来源：http://vnj.feifeiyinyue.top

arr=(a b c); echo "${arr[0]}"
来源：http://lrg.tanke756.top

[R18] 遍历数组
来源：http://hmw.cqqwz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gzl.vehdjk.com

[R19] 数组长度
来源：http://eyu.chenzaomai.com

echo "${#arr[@]}"
来源：http://yna.jqgfzy.top

[R20] 关联数组（字典）
来源：http://ldk.sufxvd.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zfo.andypj.xyz

[R21] 字符串长度
来源：http://set.pycfn.com

echo "${#s}"
来源：http://bbh.yongpay.top

[R22] 截取子串
来源：http://nao.jianghu66.top

echo "${s:0:5}"
来源：http://hhe.cqqwz.cn

[R23] 字符串替换
来源：http://mim.yfazqb.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://igd.zhixingplan.top

[R24] 大小写转换
来源：http://xfz.chenjidiqi.icu

echo "${s^^}"; echo "${s,,}"
来源：http://mxd.chenzaomai.com

[R25] 去后缀 / 去前缀
来源：http://cyw.ydjk.org.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hph.sjlbkw.cn

[R26] 命令替换
来源：http://pbq.zhoulong.xyz

now=$(date +%F); echo "$now"
来源：http://zdy.yongpay.top

[R27] 算术展开
来源：http://dav.xuanzx.com

echo $((1 + 2 * 3))
来源：http://fsf.aizwys.cn

[R28] 浮点运算
来源：http://com.guannengcc.top

echo "scale=2; 10/3" | bc
来源：http://svc.fehbvm.com

[R29] 定义函数
来源：http://qri.fehbvm.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jgt.gzhubu.top

[R30] 函数返回状态码
来源：http://ktj.yuxming.cn

f() { return 0; }; f || echo "失败了"
来源：http://nyp.zycfv.cn

[R31] 局部变量
来源：http://exw.mhx1999.top

f() { local x=1; echo "$x"; }
来源：http://jvw.zhengqikj.top

[R32] 参数个数校验
来源：http://vha.hammf.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kge.zhixingplan.top

[R33] 捕获错误并提示行号
来源：http://gcs.smart0.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mbz.bjfxy.top

[R34] 退出时清理
来源：http://wac.pycfn.com

trap 'rm -f "$tmp"' EXIT
来源：http://cok.hysaishi.cn

[R35] 后台执行并等待
来源：http://mxo.c1oappe.top

sleep 5 & pid=$!; wait "$pid"
来源：http://gwk.hnqzz.top

[R36] 并发执行多个任务
来源：http://vte.ywan-chungtsiang.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eeg.zhoulong.xyz

[R37] 把输出赋给变量
来源：http://ckc.fktsv.cn

files=$(ls -1)
来源：http://bzk.vehdjk.com

[R38] 管道串联
来源：http://orz.xuetiantiany.cn

cat a.txt | grep -i error | wc -l
来源：http://ral.bjfxy.top

[R39] 重定向标准输出与错误
来源：http://hrq.ywan-chungtsiang.top

cmd > out.log 2>&1
来源：http://sxp.ctjpmb.com

[R40] 追加写日志
来源：http://pii.cashguo.top

echo "log" >> out.log
来源：http://gwz.haohaochexian.top

[R41] 丢弃输出
来源：http://xki.nwbrower.top

cmd >/dev/null 2>&1
来源：http://fsq.zhongyouzk.top

[R42] 输入重定向
来源：http://dva.vqdsnc.cn

wc -l < a.txt
来源：http://zfn.yongpay.top

[R43] 按名字查找文件
来源：http://ahk.shuidangran.top

find . -name "*.log" -type f
来源：http://zzm.redwolf501.top

[R44] 按修改时间查找
来源：http://qsg.yangfankeji.com

find . -mtime -7 -type f
来源：http://tsp.uphjek.com

[R45] 批量删除
来源：http://pzn.jqgufenzy.top

find . -name "*.tmp" -delete
来源：http://ohr.redwolf501.top

[R46] 递归替换文件内容
来源：http://zku.nanxuanxn.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jwf.yueranfly.top

[R47] sed 单行替换
来源：http://yzc.jinqigfzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://bvg.sufxvd.cn

[R48] awk 取指定列
来源：http://ekc.cashguo.top

awk '{print $1, $3}' a.txt
来源：http://yzb.haohaochexian.top

[R49] awk 带条件
来源：http://urv.kuanghao11.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://noh.sxryk.cn

[R50] awk 求和
来源：http://hjq.xuetiantiany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://smj.jyoumei.cn

[R51] 排序去重取前几
来源：http://azn.cheryme.top

sort a.txt | uniq -c | sort -rn | head
来源：http://nvc.cdnleiting.top

[R52] 统计行数
来源：http://rxh.fktsv.cn

wc -l a.txt
来源：http://fxg.nanxuanxn.top

[R53] 查看文件头与实时尾
来源：http://reu.jiagoushi.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ybr.yuanzhike.top

[R54] 比较两个文件
来源：http://exy.zdbjq.cn

diff a.txt b.txt
来源：http://kod.yueranfly.top

[R55] 压缩与解压
来源：http://xxs.dashuyun.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zak.redwolf501.top

[R56] 远程拷贝
来源：http://oau.c1oappe.top

scp file user@host:/path/
来源：http://pvy.tianlin.xyz

[R57] 远程执行命令
来源：http://dwx.sufxvd.cn

ssh user@host 'uptime'
来源：http://dof.jyoumei.cn

[R58] 下载文件
来源：http://cix.9152youxi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wrt.uphjek.com

[R59] 发 POST JSON
来源：http://bgt.mhx1999.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ppk.hammf.cn

[R60] 只看 HTTP 状态码
来源：http://kqm.zhixingplan.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tsj.zhaomingkeji.xyz

[R61] 磁盘占用
来源：http://mry.hfpthk.cn

df -h;  du -sh *
来源：http://cyw.kuanghao11.cn

[R62] 找最占空间的文件
来源：http://zql.hcnkem.com

du -ah . | sort -rh | head -10
来源：http://sql.pycfn.com

[R63] 内存与进程
来源：http://lwf.chenzaomai.com

free -h;  ps aux | grep nginx
来源：http://ygg.cashguo.top

[R64] 结束进程
来源：http://xyb.yangfankeji.com

kill -9 $(pgrep -f app.py)
来源：http://kkx.hnqzz.top

[R65] 查看端口占用
来源：http://xgz.tarul.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://odh.fengsongda.top

[R66] 定时任务
来源：http://jdb.wangshuangyany.cn

crontab -e;  crontab -l
来源：http://wqf.redwolf501.top

[R67] 生成随机十六进制串
来源：http://amv.zdbjq.cn

openssl rand -hex 16
来源：http://cye.meibo888.top

[R68] 计算文件校验值
来源：http://yhr.ywan-chungtsiang.top

sha256sum a.txt;  md5sum a.txt
来源：http://kfs.316326.xyz

[R69] 生成随机密码
来源：http://zmx.zhengqikj.top

head -c 16 /dev/urandom | base64
来源：http://ful.hesvh.cn

[R70] 时间戳与互转
来源：http://fvb.yanxiufei.cn

date +%s;  date -d @1700000000
来源：http://mnt.9152youxi.cn

[R71] 日期格式化
来源：http://pcn.xylfe.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rxa.jinyuanbaomall.cn

[R72] 等待端口就绪
来源：http://idq.haohaochexian.top

until nc -z localhost 3306; do sleep 1; done
来源：http://lpu.nanxuanxn.top

[R73] 分割大日志
来源：http://mcn.hongshengwenyu.top

split -l 1000 big.log part_
来源：http://was.ivvv.top

[R74] 批量重命名
来源：http://bxz.fzhhl.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xdn.iojbl.cn

[R75] 导出环境变量
来源：http://jty.havefunace.top

export PATH="$HOME/bin:$PATH"
来源：http://kpe.epnwcf.com

[R76] 使用临时文件
来源：http://kuz.hywenlv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fbs.nanxinkj.top

[R77] 读取用户输入
来源：http://mmi.ehwqpu.com

read -rp "请输入: " ans
来源：http://jvc.yuxming.cn

[R78] 交互式菜单
来源：http://vsz.hcnkem.com

select opt in a b c; do echo "$opt"; break; done
来源：http://mgx.ctjpmb.com

[R79] 解析命令行选项
来源：http://klb.sxryk.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eno.dashuyun.cn

[R80] 查看脚本执行耗时
来源：http://nmf.yj202588.top

time ./run.sh
来源：http://dwq.cashguo.top

================================================================================
来源：http://ccl.hfpthk.cn

S. C / C++ 专题
来源：http://eit.jqgfzy.top

================================================================================
来源：http://jsb.vqdsnc.cn

[S01] C：Hello World
来源：http://qcp.vqdsnc.cn

#include <stdio.h>
来源：http://kbz.zdbjq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://quu.yj202588.top

[S02] C：变量与格式化输出
来源：http://xkl.zhengqikj.top

int a = 10; printf("%d\n", a);
来源：http://bve.cheryme.top

[S03] C：读入整数
来源：http://vcu.zhijiandao.cn

int x; scanf("%d", &x);
来源：http://ksd.cashguo.top

[S04] C：字符串复制
来源：http://oyy.guowangkeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://kkn.uphjek.com

[S05] C：字符串长度
来源：http://xlm.jinqigufen.top

strlen(s)
来源：http://bgj.shangyingyoupin.top

[S06] C：字符串比较
来源：http://qbx.kuanghao11.cn

strcmp(a, b) == 0
来源：http://xak.andypj.xyz

[S07] C：数组遍历求和
来源：http://xxc.9152youxi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ecw.chenjidiqi.icu

[S08] C：动态内存分配与释放
来源：http://wtn.chenzaomai.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kzn.hesvh.cn

[S09] C：结构体定义与初始化
来源：http://frs.hongshengwenyu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kht.yongpay.top

[S10] C：指针与解引用
来源：http://kqf.jlsjyb.cn

int *p = &a;  *p = 5;
来源：http://liz.fehbvm.com

[S11] C：逐行读文件
来源：http://qot.52xcode.cn

FILE *f = fopen("a.txt", "r");
来源：http://wza.jlsjyb.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qad.vqdsnc.cn

fclose(f);
来源：http://tdr.aibaodan.cn

[S12] C：写文件
来源：http://fcc.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://chl.shangyingyoupin.top

[S13] C：宏定义
来源：http://frv.aizwys.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qnl.zhaomingkeji.xyz

[S14] C：枚举
来源：http://xds.shuidangran.top

enum Color { RED, GREEN, BLUE };
来源：http://amh.jlsjyb.cn

[S15] C：类型转换
来源：http://egr.ywan-chungtsiang.top

(double) a / b
来源：http://upx.xinyue.icu

[S16] C：位操作置位
来源：http://orp.meibo888.top

x |= (1 << 3);
来源：http://fxc.jinghuilouyu.cn

[S17] C：安全拼接字符串
来源：http://vqa.tian-w.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fup.haohaochexian.top

[S18] C：命令行参数
来源：http://xih.ydzc1.top

int main(int argc, char **argv)
来源：http://spq.sufxvd.cn

[S19] C：快速排序
来源：http://sou.svipenyu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://leq.xuetiantiany.cn

[S20] C：二分查找
来源：http://fwl.jinqigfzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://akq.ctjpmb.com

[S21] C：字符类别判断
来源：http://oyx.yj20258888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cjy.jianghu66.top

[S22] C：字符串转数字
来源：http://cyf.hcnkem.com

atoi("42");  strtod("3.14", NULL);
来源：http://lvm.quarkkingdee.top

[S23] C：随机数
来源：http://ggb.tanke756.top

srand(time(NULL));  int r = rand() % 100;
来源：http://esp.ybcxt.top

[S24] C：获取本地时间
来源：http://ykd.zhaomingkeji.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bbc.nanxuanxn.top

[S25] C：内存拷贝
来源：http://nja.sysykeji.top

memcpy(dst, src, n);
来源：http://dzu.xingfuxueyuan.xyz

[S26] C：内存清零
来源：http://hwf.jiagoushi.top

memset(a, 0, sizeof a);
来源：http://wbu.zycfv.cn

[S27] C：定义常量
来源：http://ssx.vehdjk.com

const double PI = 3.14159;
来源：http://pdr.zhijiandao.cn

[S28] C：静态变量
来源：http://yxp.zycfv.cn

static int counter = 0;
来源：http://cyh.tanke756.top

[S29] C：变参函数
来源：http://mkt.snrcjt.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://liq.aizwys.cn

[S30] C：头文件保护
来源：http://uln.jqgufenzy.top

#ifndef X_H
来源：http://pih.ywan-chungtsiang.top

#define X_H
来源：http://phr.epnwcf.com

#endif
来源：http://fma.havefunace.top

[S31] C++：Hello World
来源：http://sfi.nanxinkj.top

#include <iostream>
来源：http://pkg.uphjek.com

int main() { std::cout << "Hello\n"; }
来源：http://dhk.yueranfly.top

[S32] C++：字符串
来源：http://kws.yonumen.top

std::string s = "hi";  s += "!";
来源：http://boo.shangyingyoupin.top

[S33] C++：vector 增删
来源：http://sev.zhoulong.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mzd.feifeiyinyue.top

[S34] C++：遍历 vector
来源：http://owe.bjfxy.top

for (auto &x : v) { std::cout << x; }
来源：http://pep.svipenyu.cn

[S35] C++：map
来源：http://wsg.ydzc1.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zbh.aizwys.cn

[S36] C++：unordered_map
来源：http://fzk.xinyue.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dny.uphjek.com

[S37] C++：set
来源：http://bcm.fzhhl.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://val.daria6918.cn

[S38] C++：排序
来源：http://nsx.zhengqikj.top

std::sort(v.begin(), v.end());
来源：http://nth.jqgufenzy.top

[S39] C++：自定义比较器排序
来源：http://bhx.uphjek.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oib.shangyingyoupin.top

[S40] C++：查找元素
来源：http://arb.shuidangran.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vmz.jinyuanbaomall.cn

[S41] C++：类与构造函数
来源：http://dmj.hammf.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gyo.tian-w.cn

[S42] C++：继承与虚函数
来源：http://mfa.jianghu66.top

class B : public Base { public: void f() override {} };
来源：http://bvw.jlsjyb.cn

[S43] C++：智能指针
来源：http://ijm.52xcode.cn

auto p = std::make_unique<int>(5);
来源：http://eou.hcnkem.com

[S44] C++：引用传参
来源：http://wai.shanyushiyangkeji.top

void inc(int &x) { ++x; }
来源：http://bsm.sjlbkw.cn

[S45] C++：lambda
来源：http://iag.nanxinkj.top

auto add = [](int a, int b) { return a + b; };
来源：http://bia.gogol.net.cn

[S46] C++：函数模板
来源：http://vvd.zdqjudy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://atz.chenzaomai.com

[S47] C++：结构化绑定遍历
来源：http://xwj.hesvh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tol.jyoumei.cn

[S48] C++：逐行读文件
来源：http://ers.zdqjudy.top

std::ifstream in("a.txt");  std::string line;
来源：http://nyi.guannengcc.top

while (std::getline(in, line)) { }
来源：http://oln.zhaomingkeji.xyz

[S49] C++：写文件
来源：http://coc.chenlongwang.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://evm.ybcxt.top

[S50] C++：格式化数字
来源：http://rpv.fehbvm.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uyu.sufxvd.cn

[S51] C++：显式类型转换
来源：http://lmx.aibaodan.cn

static_cast<double>(a) / b
来源：http://ihx.jinyuanbaomall.cn

[S52] C++：const 与 noexcept
来源：http://kbq.vehdjk.com

int size() const noexcept { return n_; }
来源：http://jes.cqqwz.cn

[S53] C++：移动语义
来源：http://vvb.fanxiaobao.xyz

std::vector<int> w = std::move(v);
来源：http://vnz.yonumen.top

[S54] C++：异常处理
来源：http://wrn.ybcxt.top


<!-- 参考信息 -->