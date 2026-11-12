代发 wailian999

[Q80] 字符串截取
来源：http://thn.yongpay.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uod.feifeiyinyue.top

[Q81] 字符串替换
来源：http://uum.hongshengwenyu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://opw.pycfn.com

[Q82] 字符长度与字节长度
来源：http://odz.yueranfly.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gan.hnxiangtu.top

[Q83] 大小写转换
来源：http://jak.jlsjyb.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jvp.vehdjk.com

[Q84] 去除首尾空格
来源：http://ykl.jinghuilouyu.cn

SELECT TRIM(name) FROM users;
来源：http://jhx.aibaodan.cn

[Q85] 数值取整
来源：http://fty.yj20258888.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cbn.cdnleiting.top

[Q86] 读取 JSON 字段
来源：http://eqa.fengsongda.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ulo.aibaodan.cn

[Q87] JSON 字段做条件
来源：http://lxd.xinyue.icu

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nfd.shanyushiyangtech.top

[Q88] 行转列（条件聚合）
来源：http://fmb.pycfn.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tan.jinghuilouyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tej.gogol.net.cn

[Q89] 判断表是否存在
来源：http://sfn.ywan-chungtsiang.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://teu.shuidangran.top

[Q90] 生成序号列
来源：http://qfl.tarul.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qmb.jinqigfzy.top

================================================================================
来源：http://tgp.cqqwz.cn

R. Bash 专题
来源：http://wxw.sysykeji.top

================================================================================
来源：http://osq.ydzc1.top

[R01] shebang 与严格模式
来源：http://fpc.jianghu66.top

#!/usr/bin/env bash
来源：http://obk.jinghuilouyu.cn

set -euo pipefail
来源：http://lvk.cheryme.top

[R02] 变量赋值与使用
来源：http://brf.uphjek.com

name="Tom"; echo "$name"
来源：http://bfc.jlsjyb.cn

[R03] 只读变量
来源：http://kof.chenlongwang.top

readonly PI=3.14
来源：http://prj.guannengcc.top

[R04] 位置参数
来源：http://vss.sjlbkw.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ntk.hysaishi.cn

[R05] 参数默认值
来源：http://iec.smart0.xyz

name="${1:-default}"
来源：http://zgc.meibo888.top

[R06] 判断命令是否存在
来源：http://zxo.havefunace.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zvm.yuanzhike.top

[R07] if 判断文件
来源：http://yru.fanxiaobao.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qhh.yanxiufei.cn

[R08] 数值比较
来源：http://pdz.hongshengwenyu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://kek.redwolf501.top

[R09] 字符串比较
来源：http://iuv.jyoumei.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fee.shangyingyoupin.top

[R10] 正则匹配
来源：http://svs.jinqigufen.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nbq.tanke756.top

[R11] case 多分支
来源：http://qjw.zhoulong.xyz

case "$1" in
来源：http://gqi.fzhhl.top

start) echo "启动" ;;
来源：http://qom.c1oappe.top

stop)  echo "停止" ;;
来源：http://zgu.nanxuanxn.top

*)     echo "未知命令" ;;
来源：http://ruu.yangfankeji.com

esac
来源：http://nzi.wangdashe.top

[R12] for 遍历文件
来源：http://zej.iojbl.cn

for f in *.txt; do echo "$f"; done
来源：http://rju.aibaodan.cn

[R13] for 计数循环
来源：http://xkk.shangyingyoupin.top

for i in {1..10}; do echo "$i"; done
来源：http://nru.zdbjq.cn

[R14] C 风格 for
来源：http://olm.daria6918.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nam.xingfuxueyuan.xyz

[R15] while 逐行读文件
来源：http://lgs.jianghu66.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dhw.vqdsnc.cn

[R16] until 等待条件
来源：http://aeb.svipenyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wrg.yuxming.cn

[R17] 数组定义与取值
来源：http://ygz.shangyingyoupin.top

arr=(a b c); echo "${arr[0]}"
来源：http://rgx.andypj.xyz

[R18] 遍历数组
来源：http://rzu.tianlin.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mlp.cashguo.top

[R19] 数组长度
来源：http://dhb.gotoacloud.top

echo "${#arr[@]}"
来源：http://ljv.jinyuanbaomall.cn

[R20] 关联数组（字典）
来源：http://nsv.zhixingplan.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fva.ydzc1.top

[R21] 字符串长度
来源：http://oup.cashguo.top

echo "${#s}"
来源：http://elt.chenjidiqi.icu

[R22] 截取子串
来源：http://hjy.tian-w.cn

echo "${s:0:5}"
来源：http://wsv.ybcxt.top

[R23] 字符串替换
来源：http://oyi.hfpthk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://whe.zhijiandao.cn

[R24] 大小写转换
来源：http://lmi.aizwys.cn

echo "${s^^}"; echo "${s,,}"
来源：http://reg.316326.xyz

[R25] 去后缀 / 去前缀
来源：http://csp.sysykeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://woy.xinyue.icu

[R26] 命令替换
来源：http://ksc.9152youxi.cn

now=$(date +%F); echo "$now"
来源：http://nlu.9152youxi.cn

[R27] 算术展开
来源：http://ujn.meibo888.top

echo $((1 + 2 * 3))
来源：http://vfq.gaohongyu789.top

[R28] 浮点运算
来源：http://rmg.guowangkeji.top

echo "scale=2; 10/3" | bc
来源：http://orq.jqgfzy.top

[R29] 定义函数
来源：http://bqs.havefunace.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xpt.wangdashe.top

[R30] 函数返回状态码
来源：http://dtq.bbcook.cn

f() { return 0; }; f || echo "失败了"
来源：http://rhe.xuanzx.com

[R31] 局部变量
来源：http://lem.ywan-chungtsiang.top

f() { local x=1; echo "$x"; }
来源：http://ldp.jianghu66.top

[R32] 参数个数校验
来源：http://snn.hfpthk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://upu.jinqigufen.top

[R33] 捕获错误并提示行号
来源：http://exq.hammf.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ahu.cucudq.cn

[R34] 退出时清理
来源：http://ilw.zhiwuduotai.top

trap 'rm -f "$tmp"' EXIT
来源：http://cex.hcnkem.com

[R35] 后台执行并等待
来源：http://pvv.hesvh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tjq.zdqjudy.top

[R36] 并发执行多个任务
来源：http://dgx.birdmap.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hbs.ywan-chungtsiang.top

[R37] 把输出赋给变量
来源：http://gzr.yangfankeji.com

files=$(ls -1)
来源：http://tyk.dashuyun.cn

[R38] 管道串联
来源：http://jxt.ywan-chungtsiang.top

cat a.txt | grep -i error | wc -l
来源：http://yug.xziqi.cn

[R39] 重定向标准输出与错误
来源：http://jxi.gzhubu.top

cmd > out.log 2>&1
来源：http://vgz.hysaishi.cn

[R40] 追加写日志
来源：http://czp.yuxming.cn

echo "log" >> out.log
来源：http://puu.tianlin.xyz

[R41] 丢弃输出
来源：http://vqu.yfazqb.com

cmd >/dev/null 2>&1
来源：http://esm.tanke756.top

[R42] 输入重定向
来源：http://vkf.zdbjq.cn

wc -l < a.txt
来源：http://jgd.kuanghao11.cn

[R43] 按名字查找文件
来源：http://cna.0kj1m.cn

find . -name "*.log" -type f
来源：http://irb.nanxinkj.top

[R44] 按修改时间查找
来源：http://iaf.tian-w.cn

find . -mtime -7 -type f
来源：http://kno.pengpengdd.cyou

[R45] 批量删除
来源：http://mxm.xuetiantiany.cn

find . -name "*.tmp" -delete
来源：http://dvb.daria6918.cn

[R46] 递归替换文件内容
来源：http://xfp.aizwys.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lgn.shanyushiyangkeji.top

[R47] sed 单行替换
来源：http://mam.hnxiangtu.top

sed -i 's/foo/bar/g' a.txt
来源：http://lmy.epnwcf.com

[R48] awk 取指定列
来源：http://qar.aizwys.cn

awk '{print $1, $3}' a.txt
来源：http://wxr.wangdashe.top

[R49] awk 带条件
来源：http://qkb.zdbjq.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dee.yj20258888.top

[R50] awk 求和
来源：http://tgy.yuxming.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wbc.snrcjt.cn

[R51] 排序去重取前几
来源：http://arw.jinyuanbaomall.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://atn.yj20258888.top

[R52] 统计行数
来源：http://wnr.vqdsnc.cn

wc -l a.txt
来源：http://bss.hnqzz.top

[R53] 查看文件头与实时尾
来源：http://pcs.jianghu66.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pjk.yanxiufei.cn

[R54] 比较两个文件
来源：http://hoq.yvedp.cn

diff a.txt b.txt
来源：http://kxn.hammf.cn

[R55] 压缩与解压
来源：http://zis.iojbl.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ezu.zhijiandao.cn

[R56] 远程拷贝
来源：http://umx.shanyushiyangtech.top

scp file user@host:/path/
来源：http://ntz.nanxuanxn.top

[R57] 远程执行命令
来源：http://adf.iojbl.cn

ssh user@host 'uptime'
来源：http://xgk.bjfxy.top

[R58] 下载文件
来源：http://chs.daria6918.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://shk.haohaochexian.top

[R59] 发 POST JSON
来源：http://soi.ybcxt.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fgp.52xcode.cn

[R60] 只看 HTTP 状态码
来源：http://azd.cucudq.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xqs.yj20258888.top

[R61] 磁盘占用
来源：http://bmj.yueranfly.top

df -h;  du -sh *
来源：http://qei.xylfe.cn

[R62] 找最占空间的文件
来源：http://sdv.kuanghao11.cn

du -ah . | sort -rh | head -10
来源：http://pny.gaohongyu789.top

[R63] 内存与进程
来源：http://kni.yj202588.top

free -h;  ps aux | grep nginx
来源：http://cdr.fanxiaobao.xyz

[R64] 结束进程
来源：http://akq.yuanzhike.top

kill -9 $(pgrep -f app.py)
来源：http://csy.dianchejie.cn

[R65] 查看端口占用
来源：http://xhw.pengpengdd.cyou

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://klm.cqqwz.cn

[R66] 定时任务
来源：http://ooi.shuidangran.top

crontab -e;  crontab -l
来源：http://ytu.zhiwuduotai.top

[R67] 生成随机十六进制串
来源：http://ntx.xylfe.cn

openssl rand -hex 16
来源：http://wof.dashuyun.cn

[R68] 计算文件校验值
来源：http://iud.jinghuilouyu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lfg.fzhhl.top

[R69] 生成随机密码
来源：http://wyn.sufxvd.cn

head -c 16 /dev/urandom | base64
来源：http://blt.ydjk.org.cn

[R70] 时间戳与互转
来源：http://vqt.ctjpmb.com

date +%s;  date -d @1700000000
来源：http://wxn.aibaodan.cn

[R71] 日期格式化
来源：http://fbk.cucudq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nne.haohaochexian.top

[R72] 等待端口就绪
来源：http://mbc.cheryme.top

until nc -z localhost 3306; do sleep 1; done
来源：http://kes.wangshuangyany.cn

[R73] 分割大日志
来源：http://fft.xinyue.icu

split -l 1000 big.log part_
来源：http://cdo.ctjpmb.com

[R74] 批量重命名
来源：http://uib.meibo888.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tje.chenzaomai.com

[R75] 导出环境变量
来源：http://yxi.guannengcc.top

export PATH="$HOME/bin:$PATH"
来源：http://ids.yj20258888.top

[R76] 使用临时文件
来源：http://ipn.snrcjt.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ysc.redwolf501.top

[R77] 读取用户输入
来源：http://uls.zhijiandao.cn

read -rp "请输入: " ans
来源：http://dmx.tianlin.xyz

[R78] 交互式菜单
来源：http://qhq.birdmap.top

select opt in a b c; do echo "$opt"; break; done
来源：http://cam.fengsongda.top

[R79] 解析命令行选项
来源：http://pyz.gotoacloud.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tmw.hysaishi.cn

[R80] 查看脚本执行耗时
来源：http://ixj.jinqigufen.top

time ./run.sh
来源：http://fit.tanke756.top

================================================================================
来源：http://tob.zhongyouzk.top

S. C / C++ 专题
来源：http://wmv.shangyingyoupin.top

================================================================================
来源：http://koh.birdmap.top

[S01] C：Hello World
来源：http://tzx.ivvv.top

#include <stdio.h>
来源：http://eci.yfazqb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://cid.jianghu66.top

[S02] C：变量与格式化输出
来源：http://gpe.jinqigufen.top

int a = 10; printf("%d\n", a);
来源：http://pxy.bjfxy.top

[S03] C：读入整数
来源：http://wsy.yanxiufei.cn

int x; scanf("%d", &x);
来源：http://nxq.hfpthk.cn

[S04] C：字符串复制
来源：http://lpr.svipenyu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sez.nanxuanxn.top

[S05] C：字符串长度
来源：http://pgp.jianghu66.top

strlen(s)
来源：http://xpg.ybcxt.top

[S06] C：字符串比较
来源：http://xbf.hammf.cn

strcmp(a, b) == 0
来源：http://wnd.tanke756.top

[S07] C：数组遍历求和
来源：http://adx.52xcode.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ple.yj20258.top

[S08] C：动态内存分配与释放
来源：http://cvm.hammf.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rpq.pycfn.com

[S09] C：结构体定义与初始化
来源：http://ktj.bbcook.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vdh.yuanzhike.top

[S10] C：指针与解引用
来源：http://aoz.uphjek.com

int *p = &a;  *p = 5;
来源：http://ofw.xuanzx.com

[S11] C：逐行读文件
来源：http://xdi.fktsv.cn

FILE *f = fopen("a.txt", "r");
来源：http://crp.ywan-chungtsiang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zij.daria6918.cn

fclose(f);
来源：http://lps.havefunace.top

[S12] C：写文件
来源：http://ksg.wangshuangyany.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wbn.hammf.cn

[S13] C：宏定义
来源：http://jsj.yvedp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://agt.zhongyouzk.top

[S14] C：枚举
来源：http://rgl.chenlongwang.top

enum Color { RED, GREEN, BLUE };
来源：http://ick.jqgfzy.top

[S15] C：类型转换
来源：http://uif.hfpthk.cn

(double) a / b
来源：http://aig.xingfuxueyuan.xyz

[S16] C：位操作置位
来源：http://mqp.zhongyouzk.top

x |= (1 << 3);
来源：http://bay.gotoacloud.top

[S17] C：安全拼接字符串
来源：http://evd.shzxlz.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rvd.jinghuilouyu.cn

[S18] C：命令行参数
来源：http://sqt.bjfxy.top

int main(int argc, char **argv)
来源：http://kvm.jlsjyb.cn

[S19] C：快速排序
来源：http://iov.daria6918.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jtw.cqqwz.cn

[S20] C：二分查找
来源：http://xpc.cucudq.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hkx.dashuyun.cn

[S21] C：字符类别判断
来源：http://flc.fzhhl.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fzm.daxiang520.top

[S22] C：字符串转数字
来源：http://wuo.sjlbkw.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sds.hysaishi.cn

[S23] C：随机数
来源：http://ght.chenlongwang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://asj.hcnkem.com

[S24] C：获取本地时间
来源：http://kjz.sxryk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bih.yangfankeji.com

[S25] C：内存拷贝
来源：http://rkt.andypj.xyz

memcpy(dst, src, n);
来源：http://sws.fengsongda.top

[S26] C：内存清零
来源：http://cov.ivvv.top

memset(a, 0, sizeof a);
来源：http://fab.hesvh.cn

[S27] C：定义常量
来源：http://nre.mhx1999.top

const double PI = 3.14159;
来源：http://klh.guannengcc.top

[S28] C：静态变量
来源：http://gom.yj20258.top

static int counter = 0;
来源：http://vzq.ybcxt.top

[S29] C：变参函数
来源：http://zxe.pengpengdd.cyou

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://acy.fengsongda.top

[S30] C：头文件保护
来源：http://dxa.jinqigfzy.top

#ifndef X_H
来源：http://sxi.shanyushiyangtech.top

#define X_H
来源：http://lvb.ybcxt.top

#endif
来源：http://jiq.daxiang520.top

[S31] C++：Hello World
来源：http://xqz.daria6918.cn

#include <iostream>
来源：http://gsg.ybcxt.top

int main() { std::cout << "Hello\n"; }
来源：http://ewq.sysykeji.top

[S32] C++：字符串
来源：http://zcl.jqgufenzy.top

std::string s = "hi";  s += "!";
来源：http://whe.ydzc1.top

[S33] C++：vector 增删
来源：http://jfw.sxryk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tvb.daxiang520.top

[S34] C++：遍历 vector
来源：http://cpk.pengpengdd.cyou

for (auto &x : v) { std::cout << x; }
来源：http://twc.jyoumei.cn

[S35] C++：map
来源：http://ccg.shangyingyoupin.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zjh.jiagoushi.top

[S36] C++：unordered_map
来源：http://jng.tanke756.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qqk.hammf.cn

[S37] C++：set
来源：http://lzr.shanyushiyangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xru.daxiang520.top

[S38] C++：排序
来源：http://esn.tian-w.cn

std::sort(v.begin(), v.end());
来源：http://peb.52xcode.cn

[S39] C++：自定义比较器排序
来源：http://xya.fzhhl.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qvf.yvedp.cn

[S40] C++：查找元素
来源：http://iyx.zhiwuduotai.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://reu.ydzc1.top

[S41] C++：类与构造函数
来源：http://mdd.hesvh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mww.yj202588.top

[S42] C++：继承与虚函数
来源：http://xjw.vqdsnc.cn

class B : public Base { public: void f() override {} };
来源：http://eiz.zhaomingkeji.xyz

[S43] C++：智能指针
来源：http://hmp.cashguo.top

auto p = std::make_unique<int>(5);
来源：http://huh.gzhubu.top

[S44] C++：引用传参
来源：http://nlg.xingfuxueyuan.xyz

void inc(int &x) { ++x; }
来源：http://brm.guowangkeji.top

[S45] C++：lambda
来源：http://xih.hfpthk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xvo.chenzaomai.com

[S46] C++：函数模板
来源：http://vof.chenzaomai.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kpx.ydjk.org.cn

[S47] C++：结构化绑定遍历
来源：http://kqo.jqgfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iif.yanxiufei.cn

[S48] C++：逐行读文件
来源：http://lev.kuanghao11.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lwt.hesvh.cn

while (std::getline(in, line)) { }
来源：http://qxo.xylfe.cn

[S49] C++：写文件
来源：http://wtu.yonumen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wtb.dianchejie.cn

[S50] C++：格式化数字
来源：http://kax.zhijiandao.cn


<!-- 参考信息 -->