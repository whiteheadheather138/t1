代发 wailian999

[Q78] 当前时间
来源：http://ntz.gogol.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ufd.hywenlv.cn

[Q79] 字符串拼接
来源：http://iur.shanyushiyangtech.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://udb.meibo888.top

[Q80] 字符串截取
来源：http://rip.aibaodan.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://thd.shzxlz.cn

[Q81] 字符串替换
来源：http://izw.shanyushiyangkeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ihq.zhengqikj.top

[Q82] 字符长度与字节长度
来源：http://icr.mhx1999.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nrq.chenjidiqi.icu

[Q83] 大小写转换
来源：http://yua.xingfuxueyuan.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zmi.zhoulong.xyz

[Q84] 去除首尾空格
来源：http://gut.yuxming.cn

SELECT TRIM(name) FROM users;
来源：http://nmb.fehbvm.com

[Q85] 数值取整
来源：http://bbj.yonumen.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qvh.zhijiandao.cn

[Q86] 读取 JSON 字段
来源：http://cmj.birdmap.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lbg.yvedp.cn

[Q87] JSON 字段做条件
来源：http://xpz.xziqi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jin.hysaishi.cn

[Q88] 行转列（条件聚合）
来源：http://owr.ehwqpu.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sdy.fengsongda.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jhs.yongpay.top

[Q89] 判断表是否存在
来源：http://lzp.52xcode.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ogf.tanke756.top

[Q90] 生成序号列
来源：http://agt.gogol.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ese.bbcook.cn

================================================================================
来源：http://til.haohaochexian.top

R. Bash 专题
来源：http://jsg.c1oappe.top

================================================================================
来源：http://ayf.shzxlz.cn

[R01] shebang 与严格模式
来源：http://csj.yangfankeji.com

#!/usr/bin/env bash
来源：http://pwc.zhaomingkeji.xyz

set -euo pipefail
来源：http://hng.sysykeji.top

[R02] 变量赋值与使用
来源：http://odm.fengsongda.top

name="Tom"; echo "$name"
来源：http://iqg.meibo888.top

[R03] 只读变量
来源：http://zpk.jinyuanbaomall.cn

readonly PI=3.14
来源：http://mbn.dashuyun.cn

[R04] 位置参数
来源：http://rvu.52xcode.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oct.gaohongyu789.top

[R05] 参数默认值
来源：http://evt.yueranfly.top

name="${1:-default}"
来源：http://ewb.ppjwa.cn

[R06] 判断命令是否存在
来源：http://vyc.zhoulong.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cvr.hcnkem.com

[R07] if 判断文件
来源：http://uqk.hnxiangtu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rbu.pycfn.com

[R08] 数值比较
来源：http://mik.fktsv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ggs.redwolf501.top

[R09] 字符串比较
来源：http://uxf.kuanghao11.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cys.jinqigufen.top

[R10] 正则匹配
来源：http://edf.iojbl.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dvy.xingfuxueyuan.xyz

[R11] case 多分支
来源：http://ntp.hysaishi.cn

case "$1" in
来源：http://nqj.9152youxi.cn

start) echo "启动" ;;
来源：http://buw.yuxming.cn

stop)  echo "停止" ;;
来源：http://mpj.aizwys.cn

*)     echo "未知命令" ;;
来源：http://mxw.hcnkem.com

esac
来源：http://rwa.yuxming.cn

[R12] for 遍历文件
来源：http://ljx.zhixingplan.top

for f in *.txt; do echo "$f"; done
来源：http://gpv.zdbjq.cn

[R13] for 计数循环
来源：http://eaa.tanke756.top

for i in {1..10}; do echo "$i"; done
来源：http://fzy.316326.xyz

[R14] C 风格 for
来源：http://hoh.guowangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://agd.cashguo.top

[R15] while 逐行读文件
来源：http://djr.shanyushiyangkeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sdy.hfpthk.cn

[R16] until 等待条件
来源：http://uhz.fengsongda.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gpa.fzhhl.top

[R17] 数组定义与取值
来源：http://pcm.cdnleiting.top

arr=(a b c); echo "${arr[0]}"
来源：http://eko.ywan-chungtsiang.top

[R18] 遍历数组
来源：http://wwj.hongshengwenyu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sbn.xylfe.cn

[R19] 数组长度
来源：http://tnx.guannengcc.top

echo "${#arr[@]}"
来源：http://vcl.havefunace.top

[R20] 关联数组（字典）
来源：http://zvm.andypj.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lok.nwbrower.top

[R21] 字符串长度
来源：http://ouh.wangdashe.top

echo "${#s}"
来源：http://wyk.jqgfzy.top

[R22] 截取子串
来源：http://bwl.yvedp.cn

echo "${s:0:5}"
来源：http://jxb.shangyingyoupin.top

[R23] 字符串替换
来源：http://jhr.aizwys.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sod.iojbl.cn

[R24] 大小写转换
来源：http://ppd.dianchejie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://puy.tarul.cn

[R25] 去后缀 / 去前缀
来源：http://oyz.ydzc1.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://sdu.ivvv.top

[R26] 命令替换
来源：http://xgu.xingfuxueyuan.xyz

now=$(date +%F); echo "$now"
来源：http://nya.ctjpmb.com

[R27] 算术展开
来源：http://lsp.ctjpmb.com

echo $((1 + 2 * 3))
来源：http://dhe.kuanghao11.cn

[R28] 浮点运算
来源：http://eyx.zycfv.cn

echo "scale=2; 10/3" | bc
来源：http://tcq.cucudq.cn

[R29] 定义函数
来源：http://uje.fzhhl.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tch.zycfv.cn

[R30] 函数返回状态码
来源：http://lls.sufxvd.cn

f() { return 0; }; f || echo "失败了"
来源：http://dtu.tarul.cn

[R31] 局部变量
来源：http://hsh.hywenlv.cn

f() { local x=1; echo "$x"; }
来源：http://lnr.ywan-chungtsiang.top

[R32] 参数个数校验
来源：http://ryf.yueranfly.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xio.yangfankeji.com

[R33] 捕获错误并提示行号
来源：http://gnb.tian-w.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ihp.epnwcf.com

[R34] 退出时清理
来源：http://des.sysykeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://nke.wangdashe.top

[R35] 后台执行并等待
来源：http://nmm.yj20258.top

sleep 5 & pid=$!; wait "$pid"
来源：http://tsj.zhiwuduotai.top

[R36] 并发执行多个任务
来源：http://gga.gotoacloud.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pua.sysykeji.top

[R37] 把输出赋给变量
来源：http://thz.bbcook.cn

files=$(ls -1)
来源：http://pal.iojbl.cn

[R38] 管道串联
来源：http://mmg.birdmap.top

cat a.txt | grep -i error | wc -l
来源：http://ter.ydjk.org.cn

[R39] 重定向标准输出与错误
来源：http://qor.zdqjudy.top

cmd > out.log 2>&1
来源：http://nmt.sxryk.cn

[R40] 追加写日志
来源：http://gwv.guannengcc.top

echo "log" >> out.log
来源：http://iie.zdqjudy.top

[R41] 丢弃输出
来源：http://par.svipenyu.cn

cmd >/dev/null 2>&1
来源：http://gxd.xuanzx.com

[R42] 输入重定向
来源：http://hcj.yj20258888.top

wc -l < a.txt
来源：http://irt.nanxuanxn.top

[R43] 按名字查找文件
来源：http://nwg.ydjk.org.cn

find . -name "*.log" -type f
来源：http://rwe.yj20258.top

[R44] 按修改时间查找
来源：http://kuf.fehbvm.com

find . -mtime -7 -type f
来源：http://vzp.wangdashe.top

[R45] 批量删除
来源：http://tmr.tanke756.top

find . -name "*.tmp" -delete
来源：http://uok.fengsongda.top

[R46] 递归替换文件内容
来源：http://qmp.aizwys.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://eox.jqgfzy.top

[R47] sed 单行替换
来源：http://ovj.sxryk.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fwo.jinqigufen.top

[R48] awk 取指定列
来源：http://wkz.jinqigfzy.top

awk '{print $1, $3}' a.txt
来源：http://rje.xylfe.cn

[R49] awk 带条件
来源：http://zuw.xylfe.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uru.xuetiantiany.cn

[R50] awk 求和
来源：http://pet.shangyingyoupin.top

awk '{s += $2} END {print s}' a.txt
来源：http://cfm.daxiang520.top

[R51] 排序去重取前几
来源：http://mtj.zhixingplan.top

sort a.txt | uniq -c | sort -rn | head
来源：http://lum.hcnkem.com

[R52] 统计行数
来源：http://qdu.cdnleiting.top

wc -l a.txt
来源：http://snd.sufxvd.cn

[R53] 查看文件头与实时尾
来源：http://bca.havefunace.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bkj.haohaochexian.top

[R54] 比较两个文件
来源：http://fdr.feifeiyinyue.top

diff a.txt b.txt
来源：http://ilb.ywan-chungtsiang.top

[R55] 压缩与解压
来源：http://ueg.shzxlz.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gaa.ybcxt.top

[R56] 远程拷贝
来源：http://nxe.wangshuangyany.cn

scp file user@host:/path/
来源：http://slr.pengpengdd.cyou

[R57] 远程执行命令
来源：http://cxn.jlsjyb.cn

ssh user@host 'uptime'
来源：http://suf.ppjwa.cn

[R58] 下载文件
来源：http://kdn.meibo888.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ofl.zhaomingkeji.xyz

[R59] 发 POST JSON
来源：http://uzs.jinghuilouyu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vmf.yanxiufei.cn

[R60] 只看 HTTP 状态码
来源：http://cpm.fanxiaobao.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pkv.fzhhl.top

[R61] 磁盘占用
来源：http://wri.gogol.net.cn

df -h;  du -sh *
来源：http://hws.gotoacloud.top

[R62] 找最占空间的文件
来源：http://wtd.xinyue.icu

du -ah . | sort -rh | head -10
来源：http://fbn.yongpay.top

[R63] 内存与进程
来源：http://gdi.gaohongyu789.top

free -h;  ps aux | grep nginx
来源：http://obx.daxiang520.top

[R64] 结束进程
来源：http://vom.sweek.top

kill -9 $(pgrep -f app.py)
来源：http://ilo.bjfxy.top

[R65] 查看端口占用
来源：http://dkw.shanyushiyangkeji.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dwy.mhx1999.top

[R66] 定时任务
来源：http://ydj.gogol.net.cn

crontab -e;  crontab -l
来源：http://rqz.jqgfzy.top

[R67] 生成随机十六进制串
来源：http://vij.hnqzz.top

openssl rand -hex 16
来源：http://svw.yj202588.top

[R68] 计算文件校验值
来源：http://jst.cdnleiting.top

sha256sum a.txt;  md5sum a.txt
来源：http://ztv.vehdjk.com

[R69] 生成随机密码
来源：http://eep.jinqigufen.top

head -c 16 /dev/urandom | base64
来源：http://ghj.pycfn.com

[R70] 时间戳与互转
来源：http://tgz.zhaomingkeji.xyz

date +%s;  date -d @1700000000
来源：http://qmd.xinyue.icu

[R71] 日期格式化
来源：http://kxl.fehbvm.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://xyg.cashguo.top

[R72] 等待端口就绪
来源：http://lzr.shanyushiyangkeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://rjq.smart0.xyz

[R73] 分割大日志
来源：http://sjg.fanxiaobao.xyz

split -l 1000 big.log part_
来源：http://ikx.tianlin.xyz

[R74] 批量重命名
来源：http://wrr.sufxvd.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nck.jqgfzy.top

[R75] 导出环境变量
来源：http://mno.cqqwz.cn

export PATH="$HOME/bin:$PATH"
来源：http://sdm.sweek.top

[R76] 使用临时文件
来源：http://exc.xuetiantiany.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nkg.hfpthk.cn

[R77] 读取用户输入
来源：http://lio.sjlbkw.cn

read -rp "请输入: " ans
来源：http://psb.jqgfzy.top

[R78] 交互式菜单
来源：http://eby.sjlbkw.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://frl.kuanghao11.cn

[R79] 解析命令行选项
来源：http://ztm.hywenlv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lil.hfpthk.cn

[R80] 查看脚本执行耗时
来源：http://nnu.yanxiufei.cn

time ./run.sh
来源：http://lns.shanyushiyangkeji.top

================================================================================
来源：http://aba.nanxuanxn.top

S. C / C++ 专题
来源：http://nul.hfpthk.cn

================================================================================
来源：http://fob.yonumen.top

[S01] C：Hello World
来源：http://wdq.hfpthk.cn

#include <stdio.h>
来源：http://mok.zycfv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://afh.hesvh.cn

[S02] C：变量与格式化输出
来源：http://nlk.ehwqpu.com

int a = 10; printf("%d\n", a);
来源：http://ykz.shzxlz.cn

[S03] C：读入整数
来源：http://rqa.aibaodan.cn

int x; scanf("%d", &x);
来源：http://kxv.shangyingyoupin.top

[S04] C：字符串复制
来源：http://tog.yfazqb.com

char dst[32]; strcpy(dst, "hi");
来源：http://tio.tarul.cn

[S05] C：字符串长度
来源：http://les.zhengqikj.top

strlen(s)
来源：http://rgb.shanyushiyangtech.top

[S06] C：字符串比较
来源：http://xxb.shanyushiyangkeji.top

strcmp(a, b) == 0
来源：http://gqh.cheryme.top

[S07] C：数组遍历求和
来源：http://uzc.jyoumei.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pux.yuanzhike.top

[S08] C：动态内存分配与释放
来源：http://vdq.shangyingyoupin.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lgy.zdqjudy.top

[S09] C：结构体定义与初始化
来源：http://fbx.tian-w.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ymg.jinghuilouyu.cn

[S10] C：指针与解引用
来源：http://ypu.chenjidiqi.icu

int *p = &a;  *p = 5;
来源：http://obe.shangyingyoupin.top

[S11] C：逐行读文件
来源：http://jwr.hnqzz.top

FILE *f = fopen("a.txt", "r");
来源：http://xfq.tarul.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jug.ehwqpu.com

fclose(f);
来源：http://zce.daria6918.cn

[S12] C：写文件
来源：http://txp.xingfuxueyuan.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xfz.dashuyun.cn

[S13] C：宏定义
来源：http://tgm.tanke756.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://iyl.yangfankeji.com

[S14] C：枚举
来源：http://bni.svipenyu.cn

enum Color { RED, GREEN, BLUE };
来源：http://xyz.ehwqpu.com

[S15] C：类型转换
来源：http://nch.yuxming.cn

(double) a / b
来源：http://tid.fktsv.cn

[S16] C：位操作置位
来源：http://gwy.sjlbkw.cn

x |= (1 << 3);
来源：http://xrz.jqgufenzy.top

[S17] C：安全拼接字符串
来源：http://vuw.cheryme.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bnh.zhixingplan.top

[S18] C：命令行参数
来源：http://azb.zhongyouzk.top

int main(int argc, char **argv)
来源：http://eza.jinyuanbaomall.cn

[S19] C：快速排序
来源：http://pgf.shzxlz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jsl.hongshengwenyu.top

[S20] C：二分查找
来源：http://hqn.fktsv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://etj.nanxuanxn.top

[S21] C：字符类别判断
来源：http://ruc.yongpay.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://voe.shuidangran.top

[S22] C：字符串转数字
来源：http://cwe.dianchejie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jve.yvedp.cn

[S23] C：随机数
来源：http://tvc.cdnleiting.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ccx.wangshuangyany.cn

[S24] C：获取本地时间
来源：http://qea.ctjpmb.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bsb.shuidangran.top

[S25] C：内存拷贝
来源：http://uvx.ydzc1.top

memcpy(dst, src, n);
来源：http://gmc.gogol.net.cn

[S26] C：内存清零
来源：http://eqm.nanxinkj.top

memset(a, 0, sizeof a);
来源：http://yac.sweek.top

[S27] C：定义常量
来源：http://sua.yongpay.top

const double PI = 3.14159;
来源：http://jss.gzhubu.top

[S28] C：静态变量
来源：http://zaq.zdbjq.cn

static int counter = 0;
来源：http://jbw.ppjwa.cn

[S29] C：变参函数
来源：http://ezo.daxiang520.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://unq.0kj1m.cn

[S30] C：头文件保护
来源：http://oyq.tianlin.xyz

#ifndef X_H
来源：http://nwe.vehdjk.com

#define X_H
来源：http://ide.vqdsnc.cn

#endif
来源：http://wlg.dashuyun.cn

[S31] C++：Hello World
来源：http://mgp.jyoumei.cn

#include <iostream>
来源：http://ezw.vqdsnc.cn

int main() { std::cout << "Hello\n"; }
来源：http://err.shuidangran.top

[S32] C++：字符串
来源：http://vap.yueranfly.top

std::string s = "hi";  s += "!";
来源：http://hiy.jlsjyb.cn

[S33] C++：vector 增删
来源：http://dyj.wangdashe.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eqy.shuidangran.top

[S34] C++：遍历 vector
来源：http://rbp.epnwcf.com

for (auto &x : v) { std::cout << x; }
来源：http://erl.zdbjq.cn

[S35] C++：map
来源：http://xut.xylfe.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://puv.kuanghao11.cn

[S36] C++：unordered_map
来源：http://qfi.tanke756.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mqs.316326.xyz

[S37] C++：set
来源：http://clw.yongpay.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ijv.fktsv.cn

[S38] C++：排序
来源：http://ktx.c1oappe.top

std::sort(v.begin(), v.end());
来源：http://gcu.shanyushiyangtech.top

[S39] C++：自定义比较器排序
来源：http://ugr.ivvv.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dlr.cashguo.top

[S40] C++：查找元素
来源：http://sxg.jianghu66.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gse.sufxvd.cn

[S41] C++：类与构造函数
来源：http://aea.gogol.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pon.xinyue.icu

[S42] C++：继承与虚函数
来源：http://tfg.c1oappe.top

class B : public Base { public: void f() override {} };
来源：http://pqt.iojbl.cn

[S43] C++：智能指针
来源：http://qcy.ybcxt.top

auto p = std::make_unique<int>(5);
来源：http://nhb.shzxlz.cn

[S44] C++：引用传参
来源：http://mcq.nanxuanxn.top

void inc(int &x) { ++x; }
来源：http://wle.yanxiufei.cn

[S45] C++：lambda
来源：http://tnl.gzhubu.top

auto add = [](int a, int b) { return a + b; };
来源：http://fba.sxryk.cn

[S46] C++：函数模板
来源：http://jka.hysaishi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xtz.zhaomingkeji.xyz

[S47] C++：结构化绑定遍历
来源：http://kdg.fktsv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ztd.fanxiaobao.xyz

[S48] C++：逐行读文件
来源：http://rqv.birdmap.top

std::ifstream in("a.txt");  std::string line;
来源：http://hxx.smart0.xyz


<!-- 参考信息 -->