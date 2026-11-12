代发 wailian999

[Q82] 字符长度与字节长度
来源：http://odo.andypj.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zqa.hcnkem.com

[Q83] 大小写转换
来源：http://zwu.chenjidiqi.icu

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uig.jinqigfzy.top

[Q84] 去除首尾空格
来源：http://goq.svipenyu.cn

SELECT TRIM(name) FROM users;
来源：http://jwf.hnqzz.top

[Q85] 数值取整
来源：http://gzf.cqqwz.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://frw.jiagoushi.top

[Q86] 读取 JSON 字段
来源：http://gkg.shanyushiyangtech.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://erl.andypj.xyz

[Q87] JSON 字段做条件
来源：http://swu.gogol.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xku.pycfn.com

[Q88] 行转列（条件聚合）
来源：http://kdq.cashguo.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://urc.epnwcf.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vdp.redwolf501.top

[Q89] 判断表是否存在
来源：http://kbp.quarkkingdee.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kgn.gzhubu.top

[Q90] 生成序号列
来源：http://gvx.zdqjudy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ibm.yvedp.cn

================================================================================
来源：http://zfd.yonumen.top

R. Bash 专题
来源：http://jsl.316326.xyz

================================================================================
来源：http://eld.gzhubu.top

[R01] shebang 与严格模式
来源：http://ghm.cheryme.top

#!/usr/bin/env bash
来源：http://hux.zhaomingkeji.xyz

set -euo pipefail
来源：http://rkw.jqgufenzy.top

[R02] 变量赋值与使用
来源：http://stv.shanyushiyangtech.top

name="Tom"; echo "$name"
来源：http://woh.fktsv.cn

[R03] 只读变量
来源：http://lqj.fanxiaobao.xyz

readonly PI=3.14
来源：http://rmy.ivvv.top

[R04] 位置参数
来源：http://ulp.hnxiangtu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xkw.xuetiantiany.cn

[R05] 参数默认值
来源：http://dhd.cucudq.cn

name="${1:-default}"
来源：http://xmm.redwolf501.top

[R06] 判断命令是否存在
来源：http://exg.nwbrower.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tkq.svipenyu.cn

[R07] if 判断文件
来源：http://vao.iojbl.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zib.iojbl.cn

[R08] 数值比较
来源：http://xfw.xuanzx.com

if (( a > b )); then echo "a 更大"; fi
来源：http://guv.zhiwuduotai.top

[R09] 字符串比较
来源：http://ngz.daxiang520.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wma.feifeiyinyue.top

[R10] 正则匹配
来源：http://hux.yueranfly.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sve.birdmap.top

[R11] case 多分支
来源：http://sdb.zhengqikj.top

case "$1" in
来源：http://pvd.gzhubu.top

start) echo "启动" ;;
来源：http://aog.xuetiantiany.cn

stop)  echo "停止" ;;
来源：http://qsl.zhengqikj.top

*)     echo "未知命令" ;;
来源：http://kax.nwbrower.top

esac
来源：http://pyc.gaohongyu789.top

[R12] for 遍历文件
来源：http://hfh.chenjidiqi.icu

for f in *.txt; do echo "$f"; done
来源：http://ulm.bjfxy.top

[R13] for 计数循环
来源：http://nra.sufxvd.cn

for i in {1..10}; do echo "$i"; done
来源：http://swq.dianchejie.cn

[R14] C 风格 for
来源：http://uhx.jqgfzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ita.gaohongyu789.top

[R15] while 逐行读文件
来源：http://oil.ivvv.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lth.zhoulong.xyz

[R16] until 等待条件
来源：http://mgd.c1oappe.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zhx.hnxiangtu.top

[R17] 数组定义与取值
来源：http://ioh.zycfv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oao.vqdsnc.cn

[R18] 遍历数组
来源：http://wfe.ywan-chungtsiang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wib.ehwqpu.com

[R19] 数组长度
来源：http://ncf.hfpthk.cn

echo "${#arr[@]}"
来源：http://wrd.yj202588.top

[R20] 关联数组（字典）
来源：http://tqx.feifeiyinyue.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cee.jianghu66.top

[R21] 字符串长度
来源：http://dkk.hywenlv.cn

echo "${#s}"
来源：http://tvi.hysaishi.cn

[R22] 截取子串
来源：http://cpx.ivvv.top

echo "${s:0:5}"
来源：http://rip.xuanzx.com

[R23] 字符串替换
来源：http://mlx.smart0.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rdx.zycfv.cn

[R24] 大小写转换
来源：http://znj.yuxming.cn

echo "${s^^}"; echo "${s,,}"
来源：http://azm.iojbl.cn

[R25] 去后缀 / 去前缀
来源：http://pdr.daxiang520.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dif.yj20258888.top

[R26] 命令替换
来源：http://avw.yongpay.top

now=$(date +%F); echo "$now"
来源：http://boe.redwolf501.top

[R27] 算术展开
来源：http://rig.redwolf501.top

echo $((1 + 2 * 3))
来源：http://cdn.hfpthk.cn

[R28] 浮点运算
来源：http://vxt.tianlin.xyz

echo "scale=2; 10/3" | bc
来源：http://dsz.cdnleiting.top

[R29] 定义函数
来源：http://wsn.yj20258888.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tnq.yj202588.top

[R30] 函数返回状态码
来源：http://gzd.daria6918.cn

f() { return 0; }; f || echo "失败了"
来源：http://neo.hysaishi.cn

[R31] 局部变量
来源：http://kjt.guowangkeji.top

f() { local x=1; echo "$x"; }
来源：http://ieb.yonumen.top

[R32] 参数个数校验
来源：http://ixm.xziqi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kmp.jiagoushi.top

[R33] 捕获错误并提示行号
来源：http://myq.cdnleiting.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rpy.xingfuxueyuan.xyz

[R34] 退出时清理
来源：http://fto.fanxiaobao.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://xoh.dashuyun.cn

[R35] 后台执行并等待
来源：http://ttm.jinghuilouyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wgc.feifeiyinyue.top

[R36] 并发执行多个任务
来源：http://jxd.jinyuanbaomall.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cdp.shanyushiyangkeji.top

[R37] 把输出赋给变量
来源：http://qzw.yonumen.top

files=$(ls -1)
来源：http://mau.dianchejie.cn

[R38] 管道串联
来源：http://any.yj202588.top

cat a.txt | grep -i error | wc -l
来源：http://npo.daxiang520.top

[R39] 重定向标准输出与错误
来源：http://riz.9152youxi.cn

cmd > out.log 2>&1
来源：http://gcy.nwbrower.top

[R40] 追加写日志
来源：http://idf.shzxlz.cn

echo "log" >> out.log
来源：http://yed.svipenyu.cn

[R41] 丢弃输出
来源：http://ban.mhx1999.top

cmd >/dev/null 2>&1
来源：http://ntm.fengsongda.top

[R42] 输入重定向
来源：http://pwo.jqgufenzy.top

wc -l < a.txt
来源：http://rne.yonumen.top

[R43] 按名字查找文件
来源：http://yoo.daxiang520.top

find . -name "*.log" -type f
来源：http://cch.zdbjq.cn

[R44] 按修改时间查找
来源：http://rps.ywan-chungtsiang.top

find . -mtime -7 -type f
来源：http://eqt.sweek.top

[R45] 批量删除
来源：http://ydh.hfpthk.cn

find . -name "*.tmp" -delete
来源：http://yaz.mhx1999.top

[R46] 递归替换文件内容
来源：http://rut.jqgfzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ija.sweek.top

[R47] sed 单行替换
来源：http://ram.daxiang520.top

sed -i 's/foo/bar/g' a.txt
来源：http://kuc.ivvv.top

[R48] awk 取指定列
来源：http://suu.shanyushiyangtech.top

awk '{print $1, $3}' a.txt
来源：http://asa.vqdsnc.cn

[R49] awk 带条件
来源：http://hyn.yfazqb.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iry.jqgufenzy.top

[R50] awk 求和
来源：http://rtm.pengpengdd.cyou

awk '{s += $2} END {print s}' a.txt
来源：http://rqt.aibaodan.cn

[R51] 排序去重取前几
来源：http://eel.aizwys.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yqj.shanyushiyangtech.top

[R52] 统计行数
来源：http://blq.svipenyu.cn

wc -l a.txt
来源：http://ajl.jiagoushi.top

[R53] 查看文件头与实时尾
来源：http://mnj.fanxiaobao.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ytj.jyoumei.cn

[R54] 比较两个文件
来源：http://smy.zhoulong.xyz

diff a.txt b.txt
来源：http://zzq.zhaomingkeji.xyz

[R55] 压缩与解压
来源：http://xxv.yanxiufei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bge.yfazqb.com

[R56] 远程拷贝
来源：http://bbc.quarkkingdee.top

scp file user@host:/path/
来源：http://mnf.xuetiantiany.cn

[R57] 远程执行命令
来源：http://mta.gogol.net.cn

ssh user@host 'uptime'
来源：http://ogo.svipenyu.cn

[R58] 下载文件
来源：http://xgk.gzhubu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nde.hongshengwenyu.top

[R59] 发 POST JSON
来源：http://ogl.xuanzx.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qnz.jqgfzy.top

[R60] 只看 HTTP 状态码
来源：http://xid.hnxiangtu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lgs.kuanghao11.cn

[R61] 磁盘占用
来源：http://gfr.vehdjk.com

df -h;  du -sh *
来源：http://uvu.fengsongda.top

[R62] 找最占空间的文件
来源：http://hhq.haohaochexian.top

du -ah . | sort -rh | head -10
来源：http://qdn.cdnleiting.top

[R63] 内存与进程
来源：http://izy.fktsv.cn

free -h;  ps aux | grep nginx
来源：http://hpx.zhengqikj.top

[R64] 结束进程
来源：http://fvx.nanxinkj.top

kill -9 $(pgrep -f app.py)
来源：http://nie.guannengcc.top

[R65] 查看端口占用
来源：http://zsk.xuetiantiany.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ukl.ctjpmb.com

[R66] 定时任务
来源：http://iin.svipenyu.cn

crontab -e;  crontab -l
来源：http://syi.vqdsnc.cn

[R67] 生成随机十六进制串
来源：http://xuw.tian-w.cn

openssl rand -hex 16
来源：http://ozy.dashuyun.cn

[R68] 计算文件校验值
来源：http://wua.hnxiangtu.top

sha256sum a.txt;  md5sum a.txt
来源：http://mmx.hammf.cn

[R69] 生成随机密码
来源：http://oih.zhaomingkeji.xyz

head -c 16 /dev/urandom | base64
来源：http://qrs.hesvh.cn

[R70] 时间戳与互转
来源：http://azi.hnqzz.top

date +%s;  date -d @1700000000
来源：http://sct.yvedp.cn

[R71] 日期格式化
来源：http://evq.ywan-chungtsiang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://wuq.ywan-chungtsiang.top

[R72] 等待端口就绪
来源：http://fvo.chenlongwang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ayq.vehdjk.com

[R73] 分割大日志
来源：http://sar.fengsongda.top

split -l 1000 big.log part_
来源：http://yxy.daria6918.cn

[R74] 批量重命名
来源：http://shq.havefunace.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lfb.yonumen.top

[R75] 导出环境变量
来源：http://quo.tianlin.xyz

export PATH="$HOME/bin:$PATH"
来源：http://zeq.hesvh.cn

[R76] 使用临时文件
来源：http://dyh.xinyue.icu

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hex.52xcode.cn

[R77] 读取用户输入
来源：http://fnk.fzhhl.top

read -rp "请输入: " ans
来源：http://mnz.vehdjk.com

[R78] 交互式菜单
来源：http://svu.gotoacloud.top

select opt in a b c; do echo "$opt"; break; done
来源：http://yth.pengpengdd.cyou

[R79] 解析命令行选项
来源：http://kbr.tian-w.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uvy.mhx1999.top

[R80] 查看脚本执行耗时
来源：http://pct.shanyushiyangtech.top

time ./run.sh
来源：http://nqb.jqgfzy.top

================================================================================
来源：http://mbq.mhx1999.top

S. C / C++ 专题
来源：http://paj.jqgufenzy.top

================================================================================
来源：http://myi.zhijiandao.cn

[S01] C：Hello World
来源：http://slo.aibaodan.cn

#include <stdio.h>
来源：http://wgj.bjfxy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://juy.xuetiantiany.cn

[S02] C：变量与格式化输出
来源：http://hth.meibo888.top

int a = 10; printf("%d\n", a);
来源：http://ndb.yuxming.cn

[S03] C：读入整数
来源：http://tnm.shanyushiyangkeji.top

int x; scanf("%d", &x);
来源：http://cfq.dianchejie.cn

[S04] C：字符串复制
来源：http://hjw.jinqigufen.top

char dst[32]; strcpy(dst, "hi");
来源：http://fcs.316326.xyz

[S05] C：字符串长度
来源：http://onf.cucudq.cn

strlen(s)
来源：http://lwg.shuidangran.top

[S06] C：字符串比较
来源：http://qdd.birdmap.top

strcmp(a, b) == 0
来源：http://bpf.cashguo.top

[S07] C：数组遍历求和
来源：http://vco.daxiang520.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sao.hammf.cn

[S08] C：动态内存分配与释放
来源：http://sqp.jqgfzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://elt.chenlongwang.top

[S09] C：结构体定义与初始化
来源：http://irf.aizwys.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zxi.xuanzx.com

[S10] C：指针与解引用
来源：http://fap.yongpay.top

int *p = &a;  *p = 5;
来源：http://sgn.yongpay.top

[S11] C：逐行读文件
来源：http://vif.chenjidiqi.icu

FILE *f = fopen("a.txt", "r");
来源：http://cds.sjlbkw.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://emr.ehwqpu.com

fclose(f);
来源：http://oqz.ywan-chungtsiang.top

[S12] C：写文件
来源：http://twj.zhiwuduotai.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jqj.hysaishi.cn

[S13] C：宏定义
来源：http://gbx.shanyushiyangtech.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vse.zycfv.cn

[S14] C：枚举
来源：http://zpn.gotoacloud.top

enum Color { RED, GREEN, BLUE };
来源：http://jxh.jinqigfzy.top

[S15] C：类型转换
来源：http://tzu.nanxuanxn.top

(double) a / b
来源：http://phl.nanxuanxn.top

[S16] C：位操作置位
来源：http://gdq.tianlin.xyz

x |= (1 << 3);
来源：http://pjj.birdmap.top

[S17] C：安全拼接字符串
来源：http://wny.shangyingyoupin.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yfp.hfpthk.cn

[S18] C：命令行参数
来源：http://ttm.jqgfzy.top

int main(int argc, char **argv)
来源：http://htk.jinqigfzy.top

[S19] C：快速排序
来源：http://xsu.yj20258888.top

qsort(a, n, sizeof(int), cmp);
来源：http://tpr.ywan-chungtsiang.top

[S20] C：二分查找
来源：http://ufa.ivvv.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qvr.yongpay.top

[S21] C：字符类别判断
来源：http://hxq.guowangkeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://coj.zhoulong.xyz

[S22] C：字符串转数字
来源：http://kjr.yfazqb.com

atoi("42");  strtod("3.14", NULL);
来源：http://din.daria6918.cn

[S23] C：随机数
来源：http://ila.shzxlz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ymx.smart0.xyz

[S24] C：获取本地时间
来源：http://yeb.shanyushiyangtech.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mzc.guannengcc.top

[S25] C：内存拷贝
来源：http://cay.nwbrower.top

memcpy(dst, src, n);
来源：http://jco.fehbvm.com

[S26] C：内存清零
来源：http://irp.guowangkeji.top

memset(a, 0, sizeof a);
来源：http://upe.316326.xyz

[S27] C：定义常量
来源：http://emh.cqqwz.cn

const double PI = 3.14159;
来源：http://gmr.zdbjq.cn

[S28] C：静态变量
来源：http://ipb.shuidangran.top

static int counter = 0;
来源：http://vba.xuanzx.com

[S29] C：变参函数
来源：http://dlg.xuanzx.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ijt.daria6918.cn

[S30] C：头文件保护
来源：http://vuh.xuetiantiany.cn

#ifndef X_H
来源：http://cet.shzxlz.cn

#define X_H
来源：http://dtf.jiagoushi.top

#endif
来源：http://ckq.ctjpmb.com

[S31] C++：Hello World
来源：http://fxz.wangshuangyany.cn

#include <iostream>
来源：http://oqy.yvedp.cn

int main() { std::cout << "Hello\n"; }
来源：http://zhd.jinyuanbaomall.cn

[S32] C++：字符串
来源：http://rrd.yuanzhike.top

std::string s = "hi";  s += "!";
来源：http://dmu.nwbrower.top

[S33] C++：vector 增删
来源：http://cog.zdbjq.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sjb.yuxming.cn

[S34] C++：遍历 vector
来源：http://iyv.fengsongda.top

for (auto &x : v) { std::cout << x; }
来源：http://vax.gotoacloud.top

[S35] C++：map
来源：http://mjs.hywenlv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ori.yj202588.top

[S36] C++：unordered_map
来源：http://zjc.gzhubu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://emt.hfpthk.cn

[S37] C++：set
来源：http://xgg.andypj.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oex.zhaomingkeji.xyz

[S38] C++：排序
来源：http://tqk.gogol.net.cn

std::sort(v.begin(), v.end());
来源：http://szs.jqgufenzy.top

[S39] C++：自定义比较器排序
来源：http://afx.hnqzz.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://phh.pengpengdd.cyou

[S40] C++：查找元素
来源：http://mti.sjlbkw.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://djl.ywan-chungtsiang.top

[S41] C++：类与构造函数
来源：http://cis.yanxiufei.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gxb.pycfn.com

[S42] C++：继承与虚函数
来源：http://oqn.jqgfzy.top

class B : public Base { public: void f() override {} };
来源：http://mij.zycfv.cn

[S43] C++：智能指针
来源：http://sop.meibo888.top

auto p = std::make_unique<int>(5);
来源：http://pge.nanxinkj.top

[S44] C++：引用传参
来源：http://bks.ppjwa.cn

void inc(int &x) { ++x; }
来源：http://meb.ydjk.org.cn

[S45] C++：lambda
来源：http://ywe.nwbrower.top

auto add = [](int a, int b) { return a + b; };
来源：http://vmf.ctjpmb.com

[S46] C++：函数模板
来源：http://org.uphjek.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ykq.jqgfzy.top

[S47] C++：结构化绑定遍历
来源：http://ohp.ybcxt.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fga.ivvv.top

[S48] C++：逐行读文件
来源：http://lwr.ybcxt.top

std::ifstream in("a.txt");  std::string line;
来源：http://rdv.xuanzx.com

while (std::getline(in, line)) { }
来源：http://qll.iojbl.cn

[S49] C++：写文件
来源：http://qlq.zdqjudy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zzg.hesvh.cn

[S50] C++：格式化数字
来源：http://wlt.fktsv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://imq.jianghu66.top

[S51] C++：显式类型转换
来源：http://xnt.andypj.xyz

static_cast<double>(a) / b
来源：http://dqn.yfazqb.com

[S52] C++：const 与 noexcept
来源：http://asr.xylfe.cn


<!-- 参考信息 -->