代发 wailian999

[Q80] 字符串截取
来源：http://jey.cashguo.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ctf.feifeiyinyue.top

[Q81] 字符串替换
来源：http://ltg.redwolf501.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mjy.ctjpmb.com

[Q82] 字符长度与字节长度
来源：http://lln.yueranfly.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://roi.yj20258888.top

[Q83] 大小写转换
来源：http://dfw.xuanzx.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vqm.zdqjudy.top

[Q84] 去除首尾空格
来源：http://ogn.yj20258888.top

SELECT TRIM(name) FROM users;
来源：http://vvy.yangfankeji.com

[Q85] 数值取整
来源：http://yaj.yj202588.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dmh.ctjpmb.com

[Q86] 读取 JSON 字段
来源：http://xij.tanke756.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wlj.yonumen.top

[Q87] JSON 字段做条件
来源：http://ohr.svipenyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://csl.svipenyu.cn

[Q88] 行转列（条件聚合）
来源：http://idp.mhx1999.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://svt.jinghuilouyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jdn.hongshengwenyu.top

[Q89] 判断表是否存在
来源：http://fht.wangdashe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ruj.ppjwa.cn

[Q90] 生成序号列
来源：http://dsz.fehbvm.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://exz.hywenlv.cn

================================================================================
来源：http://wqu.chenlongwang.top

R. Bash 专题
来源：http://wim.shanyushiyangkeji.top

================================================================================
来源：http://rdi.ehwqpu.com

[R01] shebang 与严格模式
来源：http://rwl.hysaishi.cn

#!/usr/bin/env bash
来源：http://gko.aizwys.cn

set -euo pipefail
来源：http://juj.yfazqb.com

[R02] 变量赋值与使用
来源：http://xpd.xziqi.cn

name="Tom"; echo "$name"
来源：http://kfk.vehdjk.com

[R03] 只读变量
来源：http://nai.birdmap.top

readonly PI=3.14
来源：http://nbw.ywan-chungtsiang.top

[R04] 位置参数
来源：http://abl.cheryme.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rgq.yfazqb.com

[R05] 参数默认值
来源：http://yok.yongpay.top

name="${1:-default}"
来源：http://uli.nwbrower.top

[R06] 判断命令是否存在
来源：http://pbi.yangfankeji.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qis.shzxlz.cn

[R07] if 判断文件
来源：http://qyv.wangdashe.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hpm.daria6918.cn

[R08] 数值比较
来源：http://dbm.cqqwz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sdu.sxryk.cn

[R09] 字符串比较
来源：http://bnc.fanxiaobao.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dqg.zhaomingkeji.xyz

[R10] 正则匹配
来源：http://hvy.bbcook.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ylb.shuidangran.top

[R11] case 多分支
来源：http://qbn.jqgfzy.top

case "$1" in
来源：http://ywj.fzhhl.top

start) echo "启动" ;;
来源：http://uzt.ydjk.org.cn

stop)  echo "停止" ;;
来源：http://wvx.kuanghao11.cn

*)     echo "未知命令" ;;
来源：http://taq.zhaomingkeji.xyz

esac
来源：http://pbe.shanyushiyangkeji.top

[R12] for 遍历文件
来源：http://ihx.haohaochexian.top

for f in *.txt; do echo "$f"; done
来源：http://vjr.jyoumei.cn

[R13] for 计数循环
来源：http://gmc.yongpay.top

for i in {1..10}; do echo "$i"; done
来源：http://cmx.zhongyouzk.top

[R14] C 风格 for
来源：http://ycl.c1oappe.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://thj.vqdsnc.cn

[R15] while 逐行读文件
来源：http://thw.9152youxi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xie.yuxming.cn

[R16] until 等待条件
来源：http://llk.fengsongda.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ucc.52xcode.cn

[R17] 数组定义与取值
来源：http://nlh.bjfxy.top

arr=(a b c); echo "${arr[0]}"
来源：http://oco.kuanghao11.cn

[R18] 遍历数组
来源：http://xai.xinyue.icu

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ykr.dianchejie.cn

[R19] 数组长度
来源：http://hzn.andypj.xyz

echo "${#arr[@]}"
来源：http://zmx.sufxvd.cn

[R20] 关联数组（字典）
来源：http://bch.ydjk.org.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xon.uphjek.com

[R21] 字符串长度
来源：http://egn.bjfxy.top

echo "${#s}"
来源：http://lxb.nwbrower.top

[R22] 截取子串
来源：http://sth.jqgufenzy.top

echo "${s:0:5}"
来源：http://gqb.0kj1m.cn

[R23] 字符串替换
来源：http://gnw.tian-w.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dou.yonumen.top

[R24] 大小写转换
来源：http://fhs.andypj.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://vsl.havefunace.top

[R25] 去后缀 / 去前缀
来源：http://rxq.gaohongyu789.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://qyh.birdmap.top

[R26] 命令替换
来源：http://qqk.sufxvd.cn

now=$(date +%F); echo "$now"
来源：http://sov.daria6918.cn

[R27] 算术展开
来源：http://ggt.nanxinkj.top

echo $((1 + 2 * 3))
来源：http://opy.guannengcc.top

[R28] 浮点运算
来源：http://fzb.chenlongwang.top

echo "scale=2; 10/3" | bc
来源：http://wvc.hysaishi.cn

[R29] 定义函数
来源：http://nnt.sjlbkw.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bad.fehbvm.com

[R30] 函数返回状态码
来源：http://wji.zhongyouzk.top

f() { return 0; }; f || echo "失败了"
来源：http://fza.yvedp.cn

[R31] 局部变量
来源：http://oox.cheryme.top

f() { local x=1; echo "$x"; }
来源：http://vmk.jinqigfzy.top

[R32] 参数个数校验
来源：http://zza.aizwys.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cpf.pycfn.com

[R33] 捕获错误并提示行号
来源：http://fdk.hnxiangtu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://quw.havefunace.top

[R34] 退出时清理
来源：http://eqd.ybcxt.top

trap 'rm -f "$tmp"' EXIT
来源：http://qdo.jinqigufen.top

[R35] 后台执行并等待
来源：http://hhq.jinyuanbaomall.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vde.0kj1m.cn

[R36] 并发执行多个任务
来源：http://daw.fktsv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cab.zhiwuduotai.top

[R37] 把输出赋给变量
来源：http://rqy.316326.xyz

files=$(ls -1)
来源：http://ycq.cdnleiting.top

[R38] 管道串联
来源：http://fsf.yuxming.cn

cat a.txt | grep -i error | wc -l
来源：http://byp.kuanghao11.cn

[R39] 重定向标准输出与错误
来源：http://hew.ppjwa.cn

cmd > out.log 2>&1
来源：http://irz.hywenlv.cn

[R40] 追加写日志
来源：http://soh.havefunace.top

echo "log" >> out.log
来源：http://jma.redwolf501.top

[R41] 丢弃输出
来源：http://qug.jianghu66.top

cmd >/dev/null 2>&1
来源：http://jyq.gaohongyu789.top

[R42] 输入重定向
来源：http://lbn.c1oappe.top

wc -l < a.txt
来源：http://yim.andypj.xyz

[R43] 按名字查找文件
来源：http://pix.cashguo.top

find . -name "*.log" -type f
来源：http://nqb.ppjwa.cn

[R44] 按修改时间查找
来源：http://hdi.shanyushiyangtech.top

find . -mtime -7 -type f
来源：http://vsv.wangshuangyany.cn

[R45] 批量删除
来源：http://lxp.jinyuanbaomall.cn

find . -name "*.tmp" -delete
来源：http://yhy.chenlongwang.top

[R46] 递归替换文件内容
来源：http://jhz.ppjwa.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pzs.fktsv.cn

[R47] sed 单行替换
来源：http://mgd.xylfe.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lst.jqgfzy.top

[R48] awk 取指定列
来源：http://xdj.fengsongda.top

awk '{print $1, $3}' a.txt
来源：http://her.jyoumei.cn

[R49] awk 带条件
来源：http://hcj.cheryme.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://smv.jianghu66.top

[R50] awk 求和
来源：http://tfg.vqdsnc.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qhk.jinyuanbaomall.cn

[R51] 排序去重取前几
来源：http://owq.xuanzx.com

sort a.txt | uniq -c | sort -rn | head
来源：http://apc.yj202588.top

[R52] 统计行数
来源：http://zkd.shangyingyoupin.top

wc -l a.txt
来源：http://rin.fehbvm.com

[R53] 查看文件头与实时尾
来源：http://ywg.aibaodan.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://orl.wangdashe.top

[R54] 比较两个文件
来源：http://ehd.yuanzhike.top

diff a.txt b.txt
来源：http://nfr.jiagoushi.top

[R55] 压缩与解压
来源：http://cck.xingfuxueyuan.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://eme.mhx1999.top

[R56] 远程拷贝
来源：http://tmf.yfazqb.com

scp file user@host:/path/
来源：http://gny.xuetiantiany.cn

[R57] 远程执行命令
来源：http://yfr.vqdsnc.cn

ssh user@host 'uptime'
来源：http://gzg.nanxinkj.top

[R58] 下载文件
来源：http://xws.ppjwa.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dvi.zhiwuduotai.top

[R59] 发 POST JSON
来源：http://usn.daria6918.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ueo.jinghuilouyu.cn

[R60] 只看 HTTP 状态码
来源：http://tjj.feifeiyinyue.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sbj.aibaodan.cn

[R61] 磁盘占用
来源：http://vng.yuanzhike.top

df -h;  du -sh *
来源：http://vud.ydjk.org.cn

[R62] 找最占空间的文件
来源：http://oxp.shangyingyoupin.top

du -ah . | sort -rh | head -10
来源：http://ubj.gogol.net.cn

[R63] 内存与进程
来源：http://lih.zdbjq.cn

free -h;  ps aux | grep nginx
来源：http://ggf.jqgfzy.top

[R64] 结束进程
来源：http://zfu.cucudq.cn

kill -9 $(pgrep -f app.py)
来源：http://mjt.bjfxy.top

[R65] 查看端口占用
来源：http://gup.nwbrower.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fnv.zhengqikj.top

[R66] 定时任务
来源：http://qon.hcnkem.com

crontab -e;  crontab -l
来源：http://cwi.shzxlz.cn

[R67] 生成随机十六进制串
来源：http://jwd.jinyuanbaomall.cn

openssl rand -hex 16
来源：http://cmf.gzhubu.top

[R68] 计算文件校验值
来源：http://itb.nwbrower.top

sha256sum a.txt;  md5sum a.txt
来源：http://gia.gzhubu.top

[R69] 生成随机密码
来源：http://hbg.zycfv.cn

head -c 16 /dev/urandom | base64
来源：http://svn.fktsv.cn

[R70] 时间戳与互转
来源：http://dco.pycfn.com

date +%s;  date -d @1700000000
来源：http://nfg.ppjwa.cn

[R71] 日期格式化
来源：http://vag.jqgufenzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xqr.pengpengdd.cyou

[R72] 等待端口就绪
来源：http://vva.hnqzz.top

until nc -z localhost 3306; do sleep 1; done
来源：http://rww.ehwqpu.com

[R73] 分割大日志
来源：http://gev.fanxiaobao.xyz

split -l 1000 big.log part_
来源：http://tya.bbcook.cn

[R74] 批量重命名
来源：http://qzr.zhongyouzk.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qwo.zhongyouzk.top

[R75] 导出环境变量
来源：http://kdl.quarkkingdee.top

export PATH="$HOME/bin:$PATH"
来源：http://znq.52xcode.cn

[R76] 使用临时文件
来源：http://eko.nwbrower.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kou.nanxuanxn.top

[R77] 读取用户输入
来源：http://ogb.yuanzhike.top

read -rp "请输入: " ans
来源：http://uft.hywenlv.cn

[R78] 交互式菜单
来源：http://cqz.yongpay.top

select opt in a b c; do echo "$opt"; break; done
来源：http://tlw.tianlin.xyz

[R79] 解析命令行选项
来源：http://nha.fktsv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mzn.fanxiaobao.xyz

[R80] 查看脚本执行耗时
来源：http://phu.yangfankeji.com

time ./run.sh
来源：http://tco.xuetiantiany.cn

================================================================================
来源：http://tnt.52xcode.cn

S. C / C++ 专题
来源：http://rbq.zhijiandao.cn

================================================================================
来源：http://udd.ydzc1.top

[S01] C：Hello World
来源：http://lae.hfpthk.cn

#include <stdio.h>
来源：http://zqo.yuanzhike.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://bbb.jinqigufen.top

[S02] C：变量与格式化输出
来源：http://twz.gotoacloud.top

int a = 10; printf("%d\n", a);
来源：http://kae.chenjidiqi.icu

[S03] C：读入整数
来源：http://adh.zhaomingkeji.xyz

int x; scanf("%d", &x);
来源：http://vxs.fehbvm.com

[S04] C：字符串复制
来源：http://qmp.fktsv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wxt.zycfv.cn

[S05] C：字符串长度
来源：http://vqj.c1oappe.top

strlen(s)
来源：http://mcl.ywan-chungtsiang.top

[S06] C：字符串比较
来源：http://qdw.aizwys.cn

strcmp(a, b) == 0
来源：http://ofi.zhongyouzk.top

[S07] C：数组遍历求和
来源：http://fow.vqdsnc.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pdm.andypj.xyz

[S08] C：动态内存分配与释放
来源：http://ebr.nanxuanxn.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lco.jianghu66.top

[S09] C：结构体定义与初始化
来源：http://dda.shanyushiyangtech.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bfm.fehbvm.com

[S10] C：指针与解引用
来源：http://kub.gaohongyu789.top

int *p = &a;  *p = 5;
来源：http://rap.haohaochexian.top

[S11] C：逐行读文件
来源：http://ejd.fanxiaobao.xyz

FILE *f = fopen("a.txt", "r");
来源：http://foy.shuidangran.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://bkx.shanyushiyangtech.top

fclose(f);
来源：http://opx.yuanzhike.top

[S12] C：写文件
来源：http://gzx.cashguo.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://axg.cqqwz.cn

[S13] C：宏定义
来源：http://blk.316326.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://msg.quarkkingdee.top

[S14] C：枚举
来源：http://wyv.fehbvm.com

enum Color { RED, GREEN, BLUE };
来源：http://ing.sjlbkw.cn

[S15] C：类型转换
来源：http://iaf.yangfankeji.com

(double) a / b
来源：http://bie.jqgfzy.top

[S16] C：位操作置位
来源：http://edt.zhengqikj.top

x |= (1 << 3);
来源：http://yyz.ydzc1.top

[S17] C：安全拼接字符串
来源：http://jfa.fengsongda.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lvk.yanxiufei.cn

[S18] C：命令行参数
来源：http://eli.quarkkingdee.top

int main(int argc, char **argv)
来源：http://vfk.zhijiandao.cn

[S19] C：快速排序
来源：http://pas.gotoacloud.top

qsort(a, n, sizeof(int), cmp);
来源：http://wyp.jlsjyb.cn

[S20] C：二分查找
来源：http://gvs.yj202588.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xks.aizwys.cn

[S21] C：字符类别判断
来源：http://rho.hfpthk.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zgo.hesvh.cn

[S22] C：字符串转数字
来源：http://tna.haohaochexian.top

atoi("42");  strtod("3.14", NULL);
来源：http://pxm.zhijiandao.cn

[S23] C：随机数
来源：http://wee.jyoumei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kbr.xinyue.icu

[S24] C：获取本地时间
来源：http://axk.bjfxy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dpv.zhiwuduotai.top

[S25] C：内存拷贝
来源：http://qop.daria6918.cn

memcpy(dst, src, n);
来源：http://cbu.aibaodan.cn

[S26] C：内存清零
来源：http://sgw.vqdsnc.cn

memset(a, 0, sizeof a);
来源：http://rkz.ydjk.org.cn

[S27] C：定义常量
来源：http://vpb.zhongyouzk.top

const double PI = 3.14159;
来源：http://jgk.hywenlv.cn

[S28] C：静态变量
来源：http://bax.jyoumei.cn

static int counter = 0;
来源：http://gjl.vqdsnc.cn

[S29] C：变参函数
来源：http://dzx.ydjk.org.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://brg.jianghu66.top

[S30] C：头文件保护
来源：http://pae.jlsjyb.cn

#ifndef X_H
来源：http://lpy.0kj1m.cn

#define X_H
来源：http://wyy.redwolf501.top

#endif
来源：http://hri.aibaodan.cn

[S31] C++：Hello World
来源：http://atb.gzhubu.top

#include <iostream>
来源：http://fjo.jiagoushi.top

int main() { std::cout << "Hello\n"; }
来源：http://nfq.xuanzx.com

[S32] C++：字符串
来源：http://you.xziqi.cn

std::string s = "hi";  s += "!";
来源：http://svj.hesvh.cn

[S33] C++：vector 增删
来源：http://cia.xziqi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nie.iojbl.cn

[S34] C++：遍历 vector
来源：http://tfr.redwolf501.top

for (auto &x : v) { std::cout << x; }
来源：http://pyx.mhx1999.top

[S35] C++：map
来源：http://tbq.zhengqikj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ygb.hesvh.cn

[S36] C++：unordered_map
来源：http://dlz.zdbjq.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://slr.jqgufenzy.top

[S37] C++：set
来源：http://hrm.ctjpmb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://glw.fzhhl.top

[S38] C++：排序
来源：http://ebj.zhoulong.xyz

std::sort(v.begin(), v.end());
来源：http://dot.snrcjt.cn

[S39] C++：自定义比较器排序
来源：http://don.ybcxt.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pyl.hnxiangtu.top

[S40] C++：查找元素
来源：http://mnj.pengpengdd.cyou

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ngs.aizwys.cn

[S41] C++：类与构造函数
来源：http://zfs.gogol.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://asb.hesvh.cn

[S42] C++：继承与虚函数
来源：http://yiw.shanyushiyangkeji.top

class B : public Base { public: void f() override {} };
来源：http://dwq.hnxiangtu.top

[S43] C++：智能指针
来源：http://vms.yj20258888.top

auto p = std::make_unique<int>(5);
来源：http://oqh.jinghuilouyu.cn

[S44] C++：引用传参
来源：http://xrr.kuanghao11.cn

void inc(int &x) { ++x; }
来源：http://ozi.tianlin.xyz

[S45] C++：lambda
来源：http://xep.hywenlv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://upy.cashguo.top

[S46] C++：函数模板
来源：http://ngr.gzhubu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nho.daxiang520.top

[S47] C++：结构化绑定遍历
来源：http://cqc.316326.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jjk.gotoacloud.top

[S48] C++：逐行读文件
来源：http://yna.ctjpmb.com

std::ifstream in("a.txt");  std::string line;
来源：http://zjw.9152youxi.cn

while (std::getline(in, line)) { }
来源：http://dbc.chenzaomai.com

[S49] C++：写文件
来源：http://dxi.0kj1m.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yqu.zycfv.cn

[S50] C++：格式化数字
来源：http://fak.gaohongyu789.top


<!-- 参考信息 -->