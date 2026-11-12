代发 wailian999

[Q82] 字符长度与字节长度
来源：http://sal.zhongyouzk.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nrg.yonumen.top

[Q83] 大小写转换
来源：http://kgr.yj20258888.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bll.shangyingyoupin.top

[Q84] 去除首尾空格
来源：http://yud.gotoacloud.top

SELECT TRIM(name) FROM users;
来源：http://nus.yueranfly.top

[Q85] 数值取整
来源：http://kie.bbcook.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vvi.sxryk.cn

[Q86] 读取 JSON 字段
来源：http://ibs.yanxiufei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jyt.pengpengdd.cyou

[Q87] JSON 字段做条件
来源：http://ydl.ctjpmb.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fbd.pycfn.com

[Q88] 行转列（条件聚合）
来源：http://syr.fktsv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lpf.ehwqpu.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ceb.svipenyu.cn

[Q89] 判断表是否存在
来源：http://ium.chenzaomai.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xuh.9152youxi.cn

[Q90] 生成序号列
来源：http://ugh.316326.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gsw.bjfxy.top

================================================================================
来源：http://lew.bbcook.cn

R. Bash 专题
来源：http://tnq.c1oappe.top

================================================================================
来源：http://eyk.sufxvd.cn

[R01] shebang 与严格模式
来源：http://ezz.xylfe.cn

#!/usr/bin/env bash
来源：http://ynw.zhongyouzk.top

set -euo pipefail
来源：http://qqc.dashuyun.cn

[R02] 变量赋值与使用
来源：http://jle.ydzc1.top

name="Tom"; echo "$name"
来源：http://nfr.meibo888.top

[R03] 只读变量
来源：http://qzk.yj20258888.top

readonly PI=3.14
来源：http://vhx.tanke756.top

[R04] 位置参数
来源：http://wcv.yangfankeji.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dqx.shanyushiyangtech.top

[R05] 参数默认值
来源：http://ddu.yanxiufei.cn

name="${1:-default}"
来源：http://bun.sxryk.cn

[R06] 判断命令是否存在
来源：http://asd.yuxming.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qmo.fanxiaobao.xyz

[R07] if 判断文件
来源：http://cxq.9152youxi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ong.vehdjk.com

[R08] 数值比较
来源：http://ekl.ivvv.top

if (( a > b )); then echo "a 更大"; fi
来源：http://fch.yj202588.top

[R09] 字符串比较
来源：http://qki.tian-w.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://grb.haohaochexian.top

[R10] 正则匹配
来源：http://wgz.yj20258888.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cbv.wangshuangyany.cn

[R11] case 多分支
来源：http://hst.fengsongda.top

case "$1" in
来源：http://bjd.yuxming.cn

start) echo "启动" ;;
来源：http://qam.nanxuanxn.top

stop)  echo "停止" ;;
来源：http://zbi.tian-w.cn

*)     echo "未知命令" ;;
来源：http://oix.jinyuanbaomall.cn

esac
来源：http://bfx.iojbl.cn

[R12] for 遍历文件
来源：http://mcj.pycfn.com

for f in *.txt; do echo "$f"; done
来源：http://uwl.zhongyouzk.top

[R13] for 计数循环
来源：http://bhr.hesvh.cn

for i in {1..10}; do echo "$i"; done
来源：http://wlx.shuidangran.top

[R14] C 风格 for
来源：http://pbn.haohaochexian.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wwa.kuanghao11.cn

[R15] while 逐行读文件
来源：http://foy.ehwqpu.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kgq.yonumen.top

[R16] until 等待条件
来源：http://ysk.jinyuanbaomall.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://duo.daria6918.cn

[R17] 数组定义与取值
来源：http://izr.hammf.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vzg.bbcook.cn

[R18] 遍历数组
来源：http://olz.yongpay.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sbh.hammf.cn

[R19] 数组长度
来源：http://rud.bjfxy.top

echo "${#arr[@]}"
来源：http://agk.jinqigfzy.top

[R20] 关联数组（字典）
来源：http://iew.gogol.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kuz.jinqigufen.top

[R21] 字符串长度
来源：http://bpq.hysaishi.cn

echo "${#s}"
来源：http://bvk.guowangkeji.top

[R22] 截取子串
来源：http://nzj.shanyushiyangtech.top

echo "${s:0:5}"
来源：http://zqy.zhongyouzk.top

[R23] 字符串替换
来源：http://etr.fktsv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mpj.cashguo.top

[R24] 大小写转换
来源：http://bby.yuanzhike.top

echo "${s^^}"; echo "${s,,}"
来源：http://prk.9152youxi.cn

[R25] 去后缀 / 去前缀
来源：http://fpr.zhengqikj.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vei.0kj1m.cn

[R26] 命令替换
来源：http://mgn.xinyue.icu

now=$(date +%F); echo "$now"
来源：http://gvi.snrcjt.cn

[R27] 算术展开
来源：http://xqi.yj202588.top

echo $((1 + 2 * 3))
来源：http://lgv.xziqi.cn

[R28] 浮点运算
来源：http://uis.jiagoushi.top

echo "scale=2; 10/3" | bc
来源：http://bpw.sjlbkw.cn

[R29] 定义函数
来源：http://zrn.tanke756.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yak.daria6918.cn

[R30] 函数返回状态码
来源：http://ddc.yj202588.top

f() { return 0; }; f || echo "失败了"
来源：http://zye.fzhhl.top

[R31] 局部变量
来源：http://kdz.dashuyun.cn

f() { local x=1; echo "$x"; }
来源：http://uzu.jiagoushi.top

[R32] 参数个数校验
来源：http://jjg.svipenyu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ygy.yj20258.top

[R33] 捕获错误并提示行号
来源：http://xsf.yuanzhike.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ipm.9152youxi.cn

[R34] 退出时清理
来源：http://pyc.jiagoushi.top

trap 'rm -f "$tmp"' EXIT
来源：http://vqx.guannengcc.top

[R35] 后台执行并等待
来源：http://xap.cashguo.top

sleep 5 & pid=$!; wait "$pid"
来源：http://kkx.cucudq.cn

[R36] 并发执行多个任务
来源：http://htu.hnxiangtu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://msm.shangyingyoupin.top

[R37] 把输出赋给变量
来源：http://fmn.zdqjudy.top

files=$(ls -1)
来源：http://kua.meibo888.top

[R38] 管道串联
来源：http://gqf.svipenyu.cn

cat a.txt | grep -i error | wc -l
来源：http://eow.epnwcf.com

[R39] 重定向标准输出与错误
来源：http://erh.hcnkem.com

cmd > out.log 2>&1
来源：http://stz.cqqwz.cn

[R40] 追加写日志
来源：http://uwd.hnqzz.top

echo "log" >> out.log
来源：http://mdi.cqqwz.cn

[R41] 丢弃输出
来源：http://usf.bjfxy.top

cmd >/dev/null 2>&1
来源：http://gku.jinghuilouyu.cn

[R42] 输入重定向
来源：http://sav.smart0.xyz

wc -l < a.txt
来源：http://bwp.xinyue.icu

[R43] 按名字查找文件
来源：http://ssf.mhx1999.top

find . -name "*.log" -type f
来源：http://nfm.dashuyun.cn

[R44] 按修改时间查找
来源：http://bzf.gogol.net.cn

find . -mtime -7 -type f
来源：http://txh.tian-w.cn

[R45] 批量删除
来源：http://yuv.jqgufenzy.top

find . -name "*.tmp" -delete
来源：http://cfa.xingfuxueyuan.xyz

[R46] 递归替换文件内容
来源：http://otj.gogol.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sai.gotoacloud.top

[R47] sed 单行替换
来源：http://xru.zhongyouzk.top

sed -i 's/foo/bar/g' a.txt
来源：http://xvj.ydjk.org.cn

[R48] awk 取指定列
来源：http://gwe.cqqwz.cn

awk '{print $1, $3}' a.txt
来源：http://ohg.zdbjq.cn

[R49] awk 带条件
来源：http://qxd.hammf.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://eui.ybcxt.top

[R50] awk 求和
来源：http://kej.nanxinkj.top

awk '{s += $2} END {print s}' a.txt
来源：http://edk.bjfxy.top

[R51] 排序去重取前几
来源：http://lpn.daxiang520.top

sort a.txt | uniq -c | sort -rn | head
来源：http://apr.ydzc1.top

[R52] 统计行数
来源：http://jiq.jiagoushi.top

wc -l a.txt
来源：http://pbg.shuidangran.top

[R53] 查看文件头与实时尾
来源：http://agb.jinqigufen.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jfr.gotoacloud.top

[R54] 比较两个文件
来源：http://kve.snrcjt.cn

diff a.txt b.txt
来源：http://zvj.zycfv.cn

[R55] 压缩与解压
来源：http://phf.ctjpmb.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uco.cheryme.top

[R56] 远程拷贝
来源：http://uwa.fanxiaobao.xyz

scp file user@host:/path/
来源：http://nmg.yj20258.top

[R57] 远程执行命令
来源：http://qqa.ehwqpu.com

ssh user@host 'uptime'
来源：http://vjl.gogol.net.cn

[R58] 下载文件
来源：http://xph.nanxinkj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qkn.xziqi.cn

[R59] 发 POST JSON
来源：http://tqy.jlsjyb.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vsv.uphjek.com

[R60] 只看 HTTP 状态码
来源：http://arw.yuxming.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kls.sysykeji.top

[R61] 磁盘占用
来源：http://rmu.bbcook.cn

df -h;  du -sh *
来源：http://grj.yanxiufei.cn

[R62] 找最占空间的文件
来源：http://jwk.vqdsnc.cn

du -ah . | sort -rh | head -10
来源：http://oge.gzhubu.top

[R63] 内存与进程
来源：http://okb.wangshuangyany.cn

free -h;  ps aux | grep nginx
来源：http://aed.guannengcc.top

[R64] 结束进程
来源：http://foz.aizwys.cn

kill -9 $(pgrep -f app.py)
来源：http://rng.tarul.cn

[R65] 查看端口占用
来源：http://zdr.nanxuanxn.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rrh.yj202588.top

[R66] 定时任务
来源：http://qfw.hammf.cn

crontab -e;  crontab -l
来源：http://iyx.haohaochexian.top

[R67] 生成随机十六进制串
来源：http://ymw.yvedp.cn

openssl rand -hex 16
来源：http://jrp.yueranfly.top

[R68] 计算文件校验值
来源：http://tsu.cucudq.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kmn.zhijiandao.cn

[R69] 生成随机密码
来源：http://etm.zhijiandao.cn

head -c 16 /dev/urandom | base64
来源：http://ksu.zdbjq.cn

[R70] 时间戳与互转
来源：http://yrs.hesvh.cn

date +%s;  date -d @1700000000
来源：http://oqk.zdbjq.cn

[R71] 日期格式化
来源：http://wkh.yueranfly.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://auu.ctjpmb.com

[R72] 等待端口就绪
来源：http://win.svipenyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://apg.nanxuanxn.top

[R73] 分割大日志
来源：http://jfr.52xcode.cn

split -l 1000 big.log part_
来源：http://kxc.meibo888.top

[R74] 批量重命名
来源：http://rpl.bjfxy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zkt.zhijiandao.cn

[R75] 导出环境变量
来源：http://ggc.wangdashe.top

export PATH="$HOME/bin:$PATH"
来源：http://ksm.daxiang520.top

[R76] 使用临时文件
来源：http://kez.pengpengdd.cyou

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://aen.cdnleiting.top

[R77] 读取用户输入
来源：http://stn.ywan-chungtsiang.top

read -rp "请输入: " ans
来源：http://pxm.aizwys.cn

[R78] 交互式菜单
来源：http://tdg.guowangkeji.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xpx.quarkkingdee.top

[R79] 解析命令行选项
来源：http://shv.vqdsnc.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xou.yvedp.cn

[R80] 查看脚本执行耗时
来源：http://hbg.jianghu66.top

time ./run.sh
来源：http://gxf.yfazqb.com

================================================================================
来源：http://unu.nanxinkj.top

S. C / C++ 专题
来源：http://szp.xuanzx.com

================================================================================
来源：http://hqp.hcnkem.com

[S01] C：Hello World
来源：http://och.gotoacloud.top

#include <stdio.h>
来源：http://skm.xuanzx.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://uzl.uphjek.com

[S02] C：变量与格式化输出
来源：http://pye.ehwqpu.com

int a = 10; printf("%d\n", a);
来源：http://mqw.jyoumei.cn

[S03] C：读入整数
来源：http://jtq.wangshuangyany.cn

int x; scanf("%d", &x);
来源：http://tri.yueranfly.top

[S04] C：字符串复制
来源：http://jxs.hywenlv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rsa.jqgfzy.top

[S05] C：字符串长度
来源：http://qww.cdnleiting.top

strlen(s)
来源：http://pes.shangyingyoupin.top

[S06] C：字符串比较
来源：http://yew.hongshengwenyu.top

strcmp(a, b) == 0
来源：http://xgb.snrcjt.cn

[S07] C：数组遍历求和
来源：http://ayw.yonumen.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://leu.zycfv.cn

[S08] C：动态内存分配与释放
来源：http://wui.nanxinkj.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kij.zhixingplan.top

[S09] C：结构体定义与初始化
来源：http://cvb.sjlbkw.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mtz.hysaishi.cn

[S10] C：指针与解引用
来源：http://txh.cdnleiting.top

int *p = &a;  *p = 5;
来源：http://nxm.xylfe.cn

[S11] C：逐行读文件
来源：http://ipw.dashuyun.cn

FILE *f = fopen("a.txt", "r");
来源：http://aum.guowangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://jkk.kuanghao11.cn

fclose(f);
来源：http://zot.hongshengwenyu.top

[S12] C：写文件
来源：http://jzc.zhaomingkeji.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gpr.hysaishi.cn

[S13] C：宏定义
来源：http://nfy.c1oappe.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ozu.pengpengdd.cyou

[S14] C：枚举
来源：http://bde.dianchejie.cn

enum Color { RED, GREEN, BLUE };
来源：http://llv.xinyue.icu

[S15] C：类型转换
来源：http://mdg.yanxiufei.cn

(double) a / b
来源：http://bko.redwolf501.top

[S16] C：位操作置位
来源：http://ugv.wangshuangyany.cn

x |= (1 << 3);
来源：http://sda.52xcode.cn

[S17] C：安全拼接字符串
来源：http://wmm.9152youxi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nlg.nanxuanxn.top

[S18] C：命令行参数
来源：http://iqc.ehwqpu.com

int main(int argc, char **argv)
来源：http://yxh.shanyushiyangkeji.top

[S19] C：快速排序
来源：http://ltl.yueranfly.top

qsort(a, n, sizeof(int), cmp);
来源：http://bph.fengsongda.top

[S20] C：二分查找
来源：http://dvd.xuetiantiany.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dak.sweek.top

[S21] C：字符类别判断
来源：http://gdo.kuanghao11.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mvc.tian-w.cn

[S22] C：字符串转数字
来源：http://adl.epnwcf.com

atoi("42");  strtod("3.14", NULL);
来源：http://wuq.hysaishi.cn

[S23] C：随机数
来源：http://ugu.nwbrower.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fpo.cashguo.top

[S24] C：获取本地时间
来源：http://syb.daxiang520.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hfx.zhixingplan.top

[S25] C：内存拷贝
来源：http://dud.hnqzz.top

memcpy(dst, src, n);
来源：http://gqs.xuetiantiany.cn

[S26] C：内存清零
来源：http://xbz.xuanzx.com

memset(a, 0, sizeof a);
来源：http://ziu.zhengqikj.top

[S27] C：定义常量
来源：http://kjy.52xcode.cn

const double PI = 3.14159;
来源：http://ypf.wangshuangyany.cn

[S28] C：静态变量
来源：http://kcq.yuxming.cn

static int counter = 0;
来源：http://bpj.tarul.cn

[S29] C：变参函数
来源：http://vhg.nanxinkj.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pkc.fktsv.cn

[S30] C：头文件保护
来源：http://lew.guannengcc.top

#ifndef X_H
来源：http://gcy.zycfv.cn

#define X_H
来源：http://mkj.cdnleiting.top

#endif
来源：http://qiz.vehdjk.com

[S31] C++：Hello World
来源：http://wgk.xziqi.cn

#include <iostream>
来源：http://adg.yj20258.top

int main() { std::cout << "Hello\n"; }
来源：http://iqd.ctjpmb.com

[S32] C++：字符串
来源：http://jsq.dianchejie.cn

std::string s = "hi";  s += "!";
来源：http://pcd.ywan-chungtsiang.top

[S33] C++：vector 增删
来源：http://zlu.jyoumei.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zhm.wangdashe.top

[S34] C++：遍历 vector
来源：http://kot.daxiang520.top

for (auto &x : v) { std::cout << x; }
来源：http://wnq.tarul.cn

[S35] C++：map
来源：http://xge.mhx1999.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jta.c1oappe.top

[S36] C++：unordered_map
来源：http://lrg.zhengqikj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wfu.cqqwz.cn

[S37] C++：set
来源：http://zem.ydjk.org.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vvm.chenlongwang.top

[S38] C++：排序
来源：http://fet.0kj1m.cn

std::sort(v.begin(), v.end());
来源：http://oec.gaohongyu789.top

[S39] C++：自定义比较器排序
来源：http://ntw.yvedp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wvd.fanxiaobao.xyz

[S40] C++：查找元素
来源：http://uwp.zhijiandao.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://diu.quarkkingdee.top

[S41] C++：类与构造函数
来源：http://czz.tian-w.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tnd.yanxiufei.cn

[S42] C++：继承与虚函数
来源：http://btb.xziqi.cn

class B : public Base { public: void f() override {} };
来源：http://rzy.ivvv.top

[S43] C++：智能指针
来源：http://ake.fktsv.cn

auto p = std::make_unique<int>(5);
来源：http://wum.jiagoushi.top

[S44] C++：引用传参
来源：http://vkx.shangyingyoupin.top

void inc(int &x) { ++x; }
来源：http://luk.bbcook.cn

[S45] C++：lambda
来源：http://qld.hammf.cn

auto add = [](int a, int b) { return a + b; };
来源：http://sqt.pengpengdd.cyou

[S46] C++：函数模板
来源：http://grz.xinyue.icu

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cis.yongpay.top

[S47] C++：结构化绑定遍历
来源：http://elz.xuanzx.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qsu.pycfn.com

[S48] C++：逐行读文件
来源：http://anv.svipenyu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://stt.fanxiaobao.xyz

while (std::getline(in, line)) { }
来源：http://qge.xuanzx.com

[S49] C++：写文件
来源：http://dxz.pengpengdd.cyou

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dop.yuxming.cn

[S50] C++：格式化数字
来源：http://min.yonumen.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yhw.yueranfly.top

[S51] C++：显式类型转换
来源：http://sob.aibaodan.cn

static_cast<double>(a) / b
来源：http://wvm.vqdsnc.cn

[S52] C++：const 与 noexcept
来源：http://xen.cheryme.top


<!-- 参考信息 -->