代发 wailian999

[Q82] 字符长度与字节长度
来源：http://iug.xziqi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://umy.hongshengwenyu.top

[Q83] 大小写转换
来源：http://oqu.gaohongyu789.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://elr.zhijiandao.cn

[Q84] 去除首尾空格
来源：http://jev.jiagoushi.top

SELECT TRIM(name) FROM users;
来源：http://wpw.jinghuilouyu.cn

[Q85] 数值取整
来源：http://jgp.shuidangran.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qjw.yj202588.top

[Q86] 读取 JSON 字段
来源：http://ypp.sweek.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hew.sjlbkw.cn

[Q87] JSON 字段做条件
来源：http://kuh.hammf.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qhj.redwolf501.top

[Q88] 行转列（条件聚合）
来源：http://mvo.cheryme.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://twj.fengsongda.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bon.hywenlv.cn

[Q89] 判断表是否存在
来源：http://ifv.sxryk.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hny.havefunace.top

[Q90] 生成序号列
来源：http://gcp.cheryme.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uiw.ydzc1.top

================================================================================
来源：http://loo.nanxinkj.top

R. Bash 专题
来源：http://mix.nanxinkj.top

================================================================================
来源：http://dfz.zycfv.cn

[R01] shebang 与严格模式
来源：http://pxc.zhengqikj.top

#!/usr/bin/env bash
来源：http://fyj.cashguo.top

set -euo pipefail
来源：http://pyn.vqdsnc.cn

[R02] 变量赋值与使用
来源：http://fjr.tian-w.cn

name="Tom"; echo "$name"
来源：http://zwn.fehbvm.com

[R03] 只读变量
来源：http://lxm.xingfuxueyuan.xyz

readonly PI=3.14
来源：http://tch.redwolf501.top

[R04] 位置参数
来源：http://lzl.yongpay.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jcx.dashuyun.cn

[R05] 参数默认值
来源：http://phj.iojbl.cn

name="${1:-default}"
来源：http://slw.tarul.cn

[R06] 判断命令是否存在
来源：http://onj.zdqjudy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xxq.jinqigufen.top

[R07] if 判断文件
来源：http://ahx.zhiwuduotai.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vaa.quarkkingdee.top

[R08] 数值比较
来源：http://xrz.svipenyu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qea.guannengcc.top

[R09] 字符串比较
来源：http://hbn.xuanzx.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xhs.fktsv.cn

[R10] 正则匹配
来源：http://kuw.yj20258.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uxq.cucudq.cn

[R11] case 多分支
来源：http://iwl.hnxiangtu.top

case "$1" in
来源：http://mmq.tianlin.xyz

start) echo "启动" ;;
来源：http://ygs.jinghuilouyu.cn

stop)  echo "停止" ;;
来源：http://dvb.yj20258888.top

*)     echo "未知命令" ;;
来源：http://ktz.snrcjt.cn

esac
来源：http://buf.ydzc1.top

[R12] for 遍历文件
来源：http://edm.yanxiufei.cn

for f in *.txt; do echo "$f"; done
来源：http://tng.vqdsnc.cn

[R13] for 计数循环
来源：http://lqd.dianchejie.cn

for i in {1..10}; do echo "$i"; done
来源：http://srh.haohaochexian.top

[R14] C 风格 for
来源：http://gos.jianghu66.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hfz.wangdashe.top

[R15] while 逐行读文件
来源：http://dwo.yj202588.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kcm.tarul.cn

[R16] until 等待条件
来源：http://tpa.zhaomingkeji.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hju.shzxlz.cn

[R17] 数组定义与取值
来源：http://hlr.feifeiyinyue.top

arr=(a b c); echo "${arr[0]}"
来源：http://ier.cdnleiting.top

[R18] 遍历数组
来源：http://ith.zhengqikj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://whq.snrcjt.cn

[R19] 数组长度
来源：http://jio.jqgufenzy.top

echo "${#arr[@]}"
来源：http://yyw.dashuyun.cn

[R20] 关联数组（字典）
来源：http://jab.jinqigufen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://guc.dashuyun.cn

[R21] 字符串长度
来源：http://kyb.jinqigfzy.top

echo "${#s}"
来源：http://dzv.andypj.xyz

[R22] 截取子串
来源：http://efq.hcnkem.com

echo "${s:0:5}"
来源：http://xep.yonumen.top

[R23] 字符串替换
来源：http://ebj.bbcook.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tra.dashuyun.cn

[R24] 大小写转换
来源：http://nad.yonumen.top

echo "${s^^}"; echo "${s,,}"
来源：http://gzx.yvedp.cn

[R25] 去后缀 / 去前缀
来源：http://bws.epnwcf.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://gcv.zycfv.cn

[R26] 命令替换
来源：http://zqg.sjlbkw.cn

now=$(date +%F); echo "$now"
来源：http://zie.ybcxt.top

[R27] 算术展开
来源：http://piv.wangdashe.top

echo $((1 + 2 * 3))
来源：http://enw.fanxiaobao.xyz

[R28] 浮点运算
来源：http://odt.shzxlz.cn

echo "scale=2; 10/3" | bc
来源：http://pmr.zdbjq.cn

[R29] 定义函数
来源：http://azm.feifeiyinyue.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vyk.smart0.xyz

[R30] 函数返回状态码
来源：http://aia.hcnkem.com

f() { return 0; }; f || echo "失败了"
来源：http://sns.jqgfzy.top

[R31] 局部变量
来源：http://zau.xuetiantiany.cn

f() { local x=1; echo "$x"; }
来源：http://cmi.bbcook.cn

[R32] 参数个数校验
来源：http://wrl.cqqwz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fio.jqgfzy.top

[R33] 捕获错误并提示行号
来源：http://raf.havefunace.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rmb.cdnleiting.top

[R34] 退出时清理
来源：http://uwt.cucudq.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vpw.0kj1m.cn

[R35] 后台执行并等待
来源：http://ehf.nanxuanxn.top

sleep 5 & pid=$!; wait "$pid"
来源：http://fcw.yonumen.top

[R36] 并发执行多个任务
来源：http://jba.ivvv.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vex.mhx1999.top

[R37] 把输出赋给变量
来源：http://faa.jqgufenzy.top

files=$(ls -1)
来源：http://jyy.nwbrower.top

[R38] 管道串联
来源：http://csa.epnwcf.com

cat a.txt | grep -i error | wc -l
来源：http://lur.aibaodan.cn

[R39] 重定向标准输出与错误
来源：http://hzk.wangdashe.top

cmd > out.log 2>&1
来源：http://cbb.kuanghao11.cn

[R40] 追加写日志
来源：http://iuc.jinqigufen.top

echo "log" >> out.log
来源：http://tid.hcnkem.com

[R41] 丢弃输出
来源：http://doh.yangfankeji.com

cmd >/dev/null 2>&1
来源：http://tti.gaohongyu789.top

[R42] 输入重定向
来源：http://bza.zhixingplan.top

wc -l < a.txt
来源：http://xjb.iojbl.cn

[R43] 按名字查找文件
来源：http://ywx.hongshengwenyu.top

find . -name "*.log" -type f
来源：http://bee.snrcjt.cn

[R44] 按修改时间查找
来源：http://ess.sjlbkw.cn

find . -mtime -7 -type f
来源：http://wdq.yj20258888.top

[R45] 批量删除
来源：http://fkl.c1oappe.top

find . -name "*.tmp" -delete
来源：http://ojr.hfpthk.cn

[R46] 递归替换文件内容
来源：http://xsu.andypj.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jif.bbcook.cn

[R47] sed 单行替换
来源：http://xjx.nanxuanxn.top

sed -i 's/foo/bar/g' a.txt
来源：http://sik.nanxinkj.top

[R48] awk 取指定列
来源：http://tvh.jlsjyb.cn

awk '{print $1, $3}' a.txt
来源：http://zbp.meibo888.top

[R49] awk 带条件
来源：http://urn.yj202588.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://usq.epnwcf.com

[R50] awk 求和
来源：http://qag.xuetiantiany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zbw.jiagoushi.top

[R51] 排序去重取前几
来源：http://cqq.jqgufenzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://fgl.0kj1m.cn

[R52] 统计行数
来源：http://ngt.yonumen.top

wc -l a.txt
来源：http://moi.zhijiandao.cn

[R53] 查看文件头与实时尾
来源：http://kwo.shuidangran.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jfp.ywan-chungtsiang.top

[R54] 比较两个文件
来源：http://wqi.fktsv.cn

diff a.txt b.txt
来源：http://uik.xuanzx.com

[R55] 压缩与解压
来源：http://dvw.jqgfzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cbz.chenlongwang.top

[R56] 远程拷贝
来源：http://gqi.wangdashe.top

scp file user@host:/path/
来源：http://ybn.hfpthk.cn

[R57] 远程执行命令
来源：http://raa.cashguo.top

ssh user@host 'uptime'
来源：http://vdc.vehdjk.com

[R58] 下载文件
来源：http://mga.zycfv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hrw.zycfv.cn

[R59] 发 POST JSON
来源：http://rcj.fengsongda.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nkw.gotoacloud.top

[R60] 只看 HTTP 状态码
来源：http://ftq.yuanzhike.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mmx.feifeiyinyue.top

[R61] 磁盘占用
来源：http://otd.9152youxi.cn

df -h;  du -sh *
来源：http://jmq.tarul.cn

[R62] 找最占空间的文件
来源：http://xxl.jinghuilouyu.cn

du -ah . | sort -rh | head -10
来源：http://fkz.iojbl.cn

[R63] 内存与进程
来源：http://zbb.jinyuanbaomall.cn

free -h;  ps aux | grep nginx
来源：http://ozm.hysaishi.cn

[R64] 结束进程
来源：http://hdg.tanke756.top

kill -9 $(pgrep -f app.py)
来源：http://rcz.nanxuanxn.top

[R65] 查看端口占用
来源：http://bii.xylfe.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mba.sufxvd.cn

[R66] 定时任务
来源：http://dqi.zhengqikj.top

crontab -e;  crontab -l
来源：http://ute.ybcxt.top

[R67] 生成随机十六进制串
来源：http://ooj.xylfe.cn

openssl rand -hex 16
来源：http://dun.shzxlz.cn

[R68] 计算文件校验值
来源：http://onn.daria6918.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vze.hywenlv.cn

[R69] 生成随机密码
来源：http://uco.nwbrower.top

head -c 16 /dev/urandom | base64
来源：http://dlv.hnqzz.top

[R70] 时间戳与互转
来源：http://rge.tanke756.top

date +%s;  date -d @1700000000
来源：http://ohi.shuidangran.top

[R71] 日期格式化
来源：http://vel.cashguo.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bwy.zycfv.cn

[R72] 等待端口就绪
来源：http://vzu.aibaodan.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jar.shanyushiyangkeji.top

[R73] 分割大日志
来源：http://bpg.shzxlz.cn

split -l 1000 big.log part_
来源：http://tld.feifeiyinyue.top

[R74] 批量重命名
来源：http://fgp.zhongyouzk.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tgr.zhiwuduotai.top

[R75] 导出环境变量
来源：http://edl.shangyingyoupin.top

export PATH="$HOME/bin:$PATH"
来源：http://str.xziqi.cn

[R76] 使用临时文件
来源：http://gqm.iojbl.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://icb.shangyingyoupin.top

[R77] 读取用户输入
来源：http://jda.sjlbkw.cn

read -rp "请输入: " ans
来源：http://ihd.zdbjq.cn

[R78] 交互式菜单
来源：http://ouc.xylfe.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bfj.yonumen.top

[R79] 解析命令行选项
来源：http://sag.feifeiyinyue.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pqd.xuanzx.com

[R80] 查看脚本执行耗时
来源：http://nlm.jinyuanbaomall.cn

time ./run.sh
来源：http://abq.yj20258.top

================================================================================
来源：http://hzw.guannengcc.top

S. C / C++ 专题
来源：http://see.ehwqpu.com

================================================================================
来源：http://ltg.hammf.cn

[S01] C：Hello World
来源：http://qja.zhengqikj.top

#include <stdio.h>
来源：http://zpo.dianchejie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kxg.gaohongyu789.top

[S02] C：变量与格式化输出
来源：http://wxq.fktsv.cn

int a = 10; printf("%d\n", a);
来源：http://smg.hesvh.cn

[S03] C：读入整数
来源：http://bqn.vehdjk.com

int x; scanf("%d", &x);
来源：http://zyk.hnqzz.top

[S04] C：字符串复制
来源：http://gjk.jqgufenzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://kpf.hnqzz.top

[S05] C：字符串长度
来源：http://cdb.yangfankeji.com

strlen(s)
来源：http://puw.shzxlz.cn

[S06] C：字符串比较
来源：http://nah.zhixingplan.top

strcmp(a, b) == 0
来源：http://eap.hongshengwenyu.top

[S07] C：数组遍历求和
来源：http://cnu.shzxlz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://geg.tanke756.top

[S08] C：动态内存分配与释放
来源：http://okn.zhijiandao.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rnw.hnxiangtu.top

[S09] C：结构体定义与初始化
来源：http://meo.gaohongyu789.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tvx.zhongyouzk.top

[S10] C：指针与解引用
来源：http://iau.shuidangran.top

int *p = &a;  *p = 5;
来源：http://xqt.hesvh.cn

[S11] C：逐行读文件
来源：http://swa.yj20258.top

FILE *f = fopen("a.txt", "r");
来源：http://zsz.yj202588.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://rdz.cucudq.cn

fclose(f);
来源：http://czs.ywan-chungtsiang.top

[S12] C：写文件
来源：http://rwb.ivvv.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://oiv.hfpthk.cn

[S13] C：宏定义
来源：http://vqz.ybcxt.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vnl.zycfv.cn

[S14] C：枚举
来源：http://uec.ybcxt.top

enum Color { RED, GREEN, BLUE };
来源：http://rqq.wangdashe.top

[S15] C：类型转换
来源：http://vjt.jyoumei.cn

(double) a / b
来源：http://uel.hnqzz.top

[S16] C：位操作置位
来源：http://tkc.redwolf501.top

x |= (1 << 3);
来源：http://yum.yuanzhike.top

[S17] C：安全拼接字符串
来源：http://wtw.9152youxi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ohf.daxiang520.top

[S18] C：命令行参数
来源：http://xxq.chenlongwang.top

int main(int argc, char **argv)
来源：http://wfs.ctjpmb.com

[S19] C：快速排序
来源：http://blw.xylfe.cn

qsort(a, n, sizeof(int), cmp);
来源：http://thv.zdqjudy.top

[S20] C：二分查找
来源：http://xpv.fehbvm.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mqj.cashguo.top

[S21] C：字符类别判断
来源：http://uwk.uphjek.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vwn.yongpay.top

[S22] C：字符串转数字
来源：http://fqf.quarkkingdee.top

atoi("42");  strtod("3.14", NULL);
来源：http://jof.jinyuanbaomall.cn

[S23] C：随机数
来源：http://ims.shzxlz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lia.hesvh.cn

[S24] C：获取本地时间
来源：http://dzi.52xcode.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rox.jinqigufen.top

[S25] C：内存拷贝
来源：http://znd.vehdjk.com

memcpy(dst, src, n);
来源：http://yob.shanyushiyangtech.top

[S26] C：内存清零
来源：http://vxu.xylfe.cn

memset(a, 0, sizeof a);
来源：http://hmx.gogol.net.cn

[S27] C：定义常量
来源：http://wsw.hysaishi.cn

const double PI = 3.14159;
来源：http://rwe.jqgfzy.top

[S28] C：静态变量
来源：http://yas.feifeiyinyue.top

static int counter = 0;
来源：http://mbu.jyoumei.cn

[S29] C：变参函数
来源：http://rbr.zhengqikj.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kmb.hcnkem.com

[S30] C：头文件保护
来源：http://wav.9152youxi.cn

#ifndef X_H
来源：http://ubl.zdqjudy.top

#define X_H
来源：http://gjk.xingfuxueyuan.xyz

#endif
来源：http://awc.hongshengwenyu.top

[S31] C++：Hello World
来源：http://jsb.ywan-chungtsiang.top

#include <iostream>
来源：http://tgx.zhixingplan.top

int main() { std::cout << "Hello\n"; }
来源：http://lzj.yfazqb.com

[S32] C++：字符串
来源：http://cft.havefunace.top

std::string s = "hi";  s += "!";
来源：http://vss.jlsjyb.cn

[S33] C++：vector 增删
来源：http://bwb.c1oappe.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vqt.hnxiangtu.top

[S34] C++：遍历 vector
来源：http://jpr.nanxinkj.top

for (auto &x : v) { std::cout << x; }
来源：http://thq.316326.xyz

[S35] C++：map
来源：http://nvt.jinqigfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://aus.yanxiufei.cn

[S36] C++：unordered_map
来源：http://mkr.fehbvm.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://evy.zdbjq.cn

[S37] C++：set
来源：http://rnx.shanyushiyangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uat.xuanzx.com

[S38] C++：排序
来源：http://jlw.jinghuilouyu.cn

std::sort(v.begin(), v.end());
来源：http://cvb.sjlbkw.cn

[S39] C++：自定义比较器排序
来源：http://lhj.cheryme.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hzt.yuanzhike.top

[S40] C++：查找元素
来源：http://foz.cdnleiting.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tca.nanxinkj.top

[S41] C++：类与构造函数
来源：http://aty.quarkkingdee.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iej.aizwys.cn

[S42] C++：继承与虚函数
来源：http://ozp.ppjwa.cn

class B : public Base { public: void f() override {} };
来源：http://fhu.jinqigufen.top

[S43] C++：智能指针
来源：http://bek.xuanzx.com

auto p = std::make_unique<int>(5);
来源：http://wwx.wangdashe.top

[S44] C++：引用传参
来源：http://zic.fktsv.cn

void inc(int &x) { ++x; }
来源：http://tew.hysaishi.cn

[S45] C++：lambda
来源：http://ksl.jinghuilouyu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yyk.ehwqpu.com

[S46] C++：函数模板
来源：http://hkh.9152youxi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ndp.bbcook.cn

[S47] C++：结构化绑定遍历
来源：http://kdn.jinqigfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wsy.yongpay.top

[S48] C++：逐行读文件
来源：http://sxr.vehdjk.com

std::ifstream in("a.txt");  std::string line;
来源：http://kkh.tian-w.cn

while (std::getline(in, line)) { }
来源：http://mtn.cucudq.cn

[S49] C++：写文件
来源：http://uhu.ywan-chungtsiang.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://irm.xinyue.icu

[S50] C++：格式化数字
来源：http://zzl.jinghuilouyu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oin.hammf.cn

[S51] C++：显式类型转换
来源：http://qxk.sxryk.cn

static_cast<double>(a) / b
来源：http://nnm.zycfv.cn

[S52] C++：const 与 noexcept
来源：http://xbz.sufxvd.cn


<!-- 参考信息 -->