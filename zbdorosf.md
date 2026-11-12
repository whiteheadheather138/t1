代发 wailian999

ROLLBACK TO sp1;
来源：http://mzy.tanke756.top

[Q69] 查看执行计划
来源：http://vmt.jiagoushi.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mla.xinyue.icu

[Q70] 更新统计信息
来源：http://qeb.uphjek.com

ANALYZE TABLE users;
来源：http://hht.zdqjudy.top

[Q71] 查看建表语句
来源：http://ruj.shangyingyoupin.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xhh.zycfv.cn

[Q72] 查看索引
来源：http://mzc.jinqigufen.top

SHOW INDEX FROM users;
来源：http://uuh.chenjidiqi.icu

[Q73] 查看表状态
来源：http://xzs.aizwys.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://asc.bbcook.cn

[Q74] 强制使用索引
来源：http://unv.yongpay.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://aoq.yanxiufei.cn

[Q75] 日期格式化
来源：http://nnx.jlsjyb.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mjh.yj20258.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qqm.ydzc1.top

[Q76] 按天统计
来源：http://dzx.hesvh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kqx.shzxlz.cn

[Q77] 时间加减
来源：http://ofw.wangdashe.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lxi.0kj1m.cn

[Q78] 当前时间
来源：http://ync.bjfxy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mqx.ydjk.org.cn

[Q79] 字符串拼接
来源：http://ukk.gotoacloud.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ork.jianghu66.top

[Q80] 字符串截取
来源：http://cha.cucudq.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dae.yj20258.top

[Q81] 字符串替换
来源：http://ipd.meibo888.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nqs.meibo888.top

[Q82] 字符长度与字节长度
来源：http://vzk.hysaishi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mbd.ehwqpu.com

[Q83] 大小写转换
来源：http://sgs.snrcjt.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ugl.gaohongyu789.top

[Q84] 去除首尾空格
来源：http://jwk.jinghuilouyu.cn

SELECT TRIM(name) FROM users;
来源：http://lak.xinyue.icu

[Q85] 数值取整
来源：http://woq.ivvv.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://edh.tianlin.xyz

[Q86] 读取 JSON 字段
来源：http://cry.yonumen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gyv.shangyingyoupin.top

[Q87] JSON 字段做条件
来源：http://lic.xziqi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kjj.shzxlz.cn

[Q88] 行转列（条件聚合）
来源：http://fhj.yanxiufei.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tbn.pengpengdd.cyou

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cia.yonumen.top

[Q89] 判断表是否存在
来源：http://wya.yvedp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fju.yonumen.top

[Q90] 生成序号列
来源：http://yrt.zhoulong.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nal.gogol.net.cn

================================================================================
来源：http://auv.fanxiaobao.xyz

R. Bash 专题
来源：http://nzt.ppjwa.cn

================================================================================
来源：http://koi.guowangkeji.top

[R01] shebang 与严格模式
来源：http://htb.yvedp.cn

#!/usr/bin/env bash
来源：http://lcj.yuxming.cn

set -euo pipefail
来源：http://xur.iojbl.cn

[R02] 变量赋值与使用
来源：http://mgy.hnqzz.top

name="Tom"; echo "$name"
来源：http://vok.hongshengwenyu.top

[R03] 只读变量
来源：http://mqh.52xcode.cn

readonly PI=3.14
来源：http://zto.sxryk.cn

[R04] 位置参数
来源：http://mnm.yj20258888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pib.jqgfzy.top

[R05] 参数默认值
来源：http://xpx.yuanzhike.top

name="${1:-default}"
来源：http://gmr.chenjidiqi.icu

[R06] 判断命令是否存在
来源：http://ddi.yj20258.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gmy.yonumen.top

[R07] if 判断文件
来源：http://nxa.cashguo.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pif.tarul.cn

[R08] 数值比较
来源：http://zfa.zdbjq.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hxo.ctjpmb.com

[R09] 字符串比较
来源：http://tft.gaohongyu789.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qrf.dashuyun.cn

[R10] 正则匹配
来源：http://qur.pengpengdd.cyou

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://muz.smart0.xyz

[R11] case 多分支
来源：http://txe.zhijiandao.cn

case "$1" in
来源：http://qwv.ivvv.top

start) echo "启动" ;;
来源：http://rjo.hammf.cn

stop)  echo "停止" ;;
来源：http://bfr.nanxinkj.top

*)     echo "未知命令" ;;
来源：http://ykz.mhx1999.top

esac
来源：http://pfu.52xcode.cn

[R12] for 遍历文件
来源：http://bbs.xuanzx.com

for f in *.txt; do echo "$f"; done
来源：http://rlj.ywan-chungtsiang.top

[R13] for 计数循环
来源：http://npi.gogol.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://glb.hfpthk.cn

[R14] C 风格 for
来源：http://soq.yongpay.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jnw.316326.xyz

[R15] while 逐行读文件
来源：http://upv.uphjek.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qts.chenzaomai.com

[R16] until 等待条件
来源：http://rik.guowangkeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qey.52xcode.cn

[R17] 数组定义与取值
来源：http://whw.fehbvm.com

arr=(a b c); echo "${arr[0]}"
来源：http://ejj.hysaishi.cn

[R18] 遍历数组
来源：http://evc.tanke756.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.ybcxt.top

[R19] 数组长度
来源：http://jka.bjfxy.top

echo "${#arr[@]}"
来源：http://nbn.cdnleiting.top

[R20] 关联数组（字典）
来源：http://xld.hongshengwenyu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tky.snrcjt.cn

[R21] 字符串长度
来源：http://ngb.shanyushiyangkeji.top

echo "${#s}"
来源：http://yvi.cashguo.top

[R22] 截取子串
来源：http://qru.sysykeji.top

echo "${s:0:5}"
来源：http://yhp.gaohongyu789.top

[R23] 字符串替换
来源：http://erf.bjfxy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kgi.smart0.xyz

[R24] 大小写转换
来源：http://ikz.daria6918.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zre.snrcjt.cn

[R25] 去后缀 / 去前缀
来源：http://zug.shanyushiyangtech.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://tpx.fzhhl.top

[R26] 命令替换
来源：http://zyn.jianghu66.top

now=$(date +%F); echo "$now"
来源：http://cnd.hcnkem.com

[R27] 算术展开
来源：http://kzq.zhijiandao.cn

echo $((1 + 2 * 3))
来源：http://acl.yangfankeji.com

[R28] 浮点运算
来源：http://wtu.feifeiyinyue.top

echo "scale=2; 10/3" | bc
来源：http://vtx.hnqzz.top

[R29] 定义函数
来源：http://scr.guannengcc.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jdi.nanxinkj.top

[R30] 函数返回状态码
来源：http://qix.ywan-chungtsiang.top

f() { return 0; }; f || echo "失败了"
来源：http://ywp.yueranfly.top

[R31] 局部变量
来源：http://txs.hywenlv.cn

f() { local x=1; echo "$x"; }
来源：http://kke.hfpthk.cn

[R32] 参数个数校验
来源：http://kfw.smart0.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://caa.yvedp.cn

[R33] 捕获错误并提示行号
来源：http://tlf.vqdsnc.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lew.hnqzz.top

[R34] 退出时清理
来源：http://uou.chenlongwang.top

trap 'rm -f "$tmp"' EXIT
来源：http://rtq.tianlin.xyz

[R35] 后台执行并等待
来源：http://tui.zhoulong.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://qbv.tanke756.top

[R36] 并发执行多个任务
来源：http://xhg.aizwys.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qzf.jinqigufen.top

[R37] 把输出赋给变量
来源：http://sli.jlsjyb.cn

files=$(ls -1)
来源：http://nxs.aizwys.cn

[R38] 管道串联
来源：http://kzc.yueranfly.top

cat a.txt | grep -i error | wc -l
来源：http://ozy.ehwqpu.com

[R39] 重定向标准输出与错误
来源：http://zpd.cashguo.top

cmd > out.log 2>&1
来源：http://trh.zhoulong.xyz

[R40] 追加写日志
来源：http://fxg.0kj1m.cn

echo "log" >> out.log
来源：http://cds.yj20258888.top

[R41] 丢弃输出
来源：http://zjf.gaohongyu789.top

cmd >/dev/null 2>&1
来源：http://ymx.hammf.cn

[R42] 输入重定向
来源：http://lxz.yfazqb.com

wc -l < a.txt
来源：http://nhk.yj20258.top

[R43] 按名字查找文件
来源：http://wca.cashguo.top

find . -name "*.log" -type f
来源：http://wke.nanxinkj.top

[R44] 按修改时间查找
来源：http://dwl.vehdjk.com

find . -mtime -7 -type f
来源：http://pix.hfpthk.cn

[R45] 批量删除
来源：http://qiw.jlsjyb.cn

find . -name "*.tmp" -delete
来源：http://fly.zhengqikj.top

[R46] 递归替换文件内容
来源：http://uqi.jqgufenzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hkb.hfpthk.cn

[R47] sed 单行替换
来源：http://ygh.guannengcc.top

sed -i 's/foo/bar/g' a.txt
来源：http://jhc.guowangkeji.top

[R48] awk 取指定列
来源：http://phd.cucudq.cn

awk '{print $1, $3}' a.txt
来源：http://yxh.xinyue.icu

[R49] awk 带条件
来源：http://jny.quarkkingdee.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hbu.jqgufenzy.top

[R50] awk 求和
来源：http://vfa.cashguo.top

awk '{s += $2} END {print s}' a.txt
来源：http://oji.shzxlz.cn

[R51] 排序去重取前几
来源：http://hsp.guannengcc.top

sort a.txt | uniq -c | sort -rn | head
来源：http://znm.redwolf501.top

[R52] 统计行数
来源：http://wih.jianghu66.top

wc -l a.txt
来源：http://nzj.haohaochexian.top

[R53] 查看文件头与实时尾
来源：http://may.zhiwuduotai.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rcu.316326.xyz

[R54] 比较两个文件
来源：http://zsz.ydjk.org.cn

diff a.txt b.txt
来源：http://gko.zhengqikj.top

[R55] 压缩与解压
来源：http://hbf.aizwys.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://esd.epnwcf.com

[R56] 远程拷贝
来源：http://rqx.cucudq.cn

scp file user@host:/path/
来源：http://udy.fehbvm.com

[R57] 远程执行命令
来源：http://tmp.zycfv.cn

ssh user@host 'uptime'
来源：http://urj.shangyingyoupin.top

[R58] 下载文件
来源：http://myf.xuetiantiany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kjo.daxiang520.top

[R59] 发 POST JSON
来源：http://dlr.cucudq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zso.wangshuangyany.cn

[R60] 只看 HTTP 状态码
来源：http://xnj.xziqi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hga.yj20258.top

[R61] 磁盘占用
来源：http://xnw.fktsv.cn

df -h;  du -sh *
来源：http://nvi.zhiwuduotai.top

[R62] 找最占空间的文件
来源：http://ifh.nanxinkj.top

du -ah . | sort -rh | head -10
来源：http://efh.vehdjk.com

[R63] 内存与进程
来源：http://cog.jinqigufen.top

free -h;  ps aux | grep nginx
来源：http://bdz.shanyushiyangkeji.top

[R64] 结束进程
来源：http://vtb.tian-w.cn

kill -9 $(pgrep -f app.py)
来源：http://gyg.gotoacloud.top

[R65] 查看端口占用
来源：http://fqx.jinqigfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://osy.sxryk.cn

[R66] 定时任务
来源：http://dzx.sweek.top

crontab -e;  crontab -l
来源：http://wnl.jinyuanbaomall.cn

[R67] 生成随机十六进制串
来源：http://ecl.shangyingyoupin.top

openssl rand -hex 16
来源：http://uet.hnxiangtu.top

[R68] 计算文件校验值
来源：http://xxr.ctjpmb.com

sha256sum a.txt;  md5sum a.txt
来源：http://yon.hnqzz.top

[R69] 生成随机密码
来源：http://oer.feifeiyinyue.top

head -c 16 /dev/urandom | base64
来源：http://dav.nanxuanxn.top

[R70] 时间戳与互转
来源：http://yte.zdqjudy.top

date +%s;  date -d @1700000000
来源：http://zze.zycfv.cn

[R71] 日期格式化
来源：http://ura.gzhubu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bek.ctjpmb.com

[R72] 等待端口就绪
来源：http://ewf.zhengqikj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ifa.hysaishi.cn

[R73] 分割大日志
来源：http://itl.gaohongyu789.top

split -l 1000 big.log part_
来源：http://cvi.xuanzx.com

[R74] 批量重命名
来源：http://hed.shangyingyoupin.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cgv.vehdjk.com

[R75] 导出环境变量
来源：http://ujx.tian-w.cn

export PATH="$HOME/bin:$PATH"
来源：http://ydu.ybcxt.top

[R76] 使用临时文件
来源：http://eyn.yonumen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nwj.hesvh.cn

[R77] 读取用户输入
来源：http://zai.smart0.xyz

read -rp "请输入: " ans
来源：http://hnz.nwbrower.top

[R78] 交互式菜单
来源：http://qwj.xinyue.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://ggo.hnqzz.top

[R79] 解析命令行选项
来源：http://sfl.sweek.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fpy.jinyuanbaomall.cn

[R80] 查看脚本执行耗时
来源：http://jrc.jinghuilouyu.cn

time ./run.sh
来源：http://yeu.zdbjq.cn

================================================================================
来源：http://cki.bjfxy.top

S. C / C++ 专题
来源：http://vmn.yj20258.top

================================================================================
来源：http://zas.cucudq.cn

[S01] C：Hello World
来源：http://yox.iojbl.cn

#include <stdio.h>
来源：http://xvx.sysykeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://txi.ybcxt.top

[S02] C：变量与格式化输出
来源：http://kkk.c1oappe.top

int a = 10; printf("%d\n", a);
来源：http://jbg.yuxming.cn

[S03] C：读入整数
来源：http://frw.haohaochexian.top

int x; scanf("%d", &x);
来源：http://oni.jinqigfzy.top

[S04] C：字符串复制
来源：http://lqo.ppjwa.cn

char dst[32]; strcpy(dst, "hi");
来源：http://knd.jqgfzy.top

[S05] C：字符串长度
来源：http://wrf.xuetiantiany.cn

strlen(s)
来源：http://iju.birdmap.top

[S06] C：字符串比较
来源：http://jum.fzhhl.top

strcmp(a, b) == 0
来源：http://mjc.tian-w.cn

[S07] C：数组遍历求和
来源：http://zyy.yvedp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zyv.guannengcc.top

[S08] C：动态内存分配与释放
来源：http://tzw.chenjidiqi.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ahm.zhoulong.xyz

[S09] C：结构体定义与初始化
来源：http://vxt.aizwys.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kkk.zhaomingkeji.xyz

[S10] C：指针与解引用
来源：http://yuq.jyoumei.cn

int *p = &a;  *p = 5;
来源：http://hrj.snrcjt.cn

[S11] C：逐行读文件
来源：http://ngi.nwbrower.top

FILE *f = fopen("a.txt", "r");
来源：http://wvx.tianlin.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://wlm.birdmap.top

fclose(f);
来源：http://xui.nanxuanxn.top

[S12] C：写文件
来源：http://cyx.havefunace.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yfp.zdqjudy.top

[S13] C：宏定义
来源：http://ojq.bbcook.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://szz.sufxvd.cn

[S14] C：枚举
来源：http://ytl.xuetiantiany.cn

enum Color { RED, GREEN, BLUE };
来源：http://wxp.nanxinkj.top

[S15] C：类型转换
来源：http://ana.cucudq.cn

(double) a / b
来源：http://hay.xinyue.icu

[S16] C：位操作置位
来源：http://qfe.andypj.xyz

x |= (1 << 3);
来源：http://baw.nwbrower.top

[S17] C：安全拼接字符串
来源：http://wev.ydzc1.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lvg.wangdashe.top

[S18] C：命令行参数
来源：http://uee.zhoulong.xyz

int main(int argc, char **argv)
来源：http://lpl.zycfv.cn

[S19] C：快速排序
来源：http://ejq.gaohongyu789.top

qsort(a, n, sizeof(int), cmp);
来源：http://bmq.sysykeji.top

[S20] C：二分查找
来源：http://uot.vehdjk.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vtf.tarul.cn

[S21] C：字符类别判断
来源：http://ftt.dashuyun.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ipa.hywenlv.cn

[S22] C：字符串转数字
来源：http://ieb.ehwqpu.com

atoi("42");  strtod("3.14", NULL);
来源：http://tzw.daxiang520.top

[S23] C：随机数
来源：http://eve.gaohongyu789.top

srand(time(NULL));  int r = rand() % 100;
来源：http://hik.bjfxy.top

[S24] C：获取本地时间
来源：http://dsy.gzhubu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mkf.andypj.xyz

[S25] C：内存拷贝
来源：http://zka.316326.xyz

memcpy(dst, src, n);
来源：http://uef.hongshengwenyu.top

[S26] C：内存清零
来源：http://whe.andypj.xyz

memset(a, 0, sizeof a);
来源：http://ths.nanxinkj.top

[S27] C：定义常量
来源：http://uyp.sxryk.cn

const double PI = 3.14159;
来源：http://twt.fanxiaobao.xyz

[S28] C：静态变量
来源：http://ejt.fengsongda.top

static int counter = 0;
来源：http://srv.havefunace.top

[S29] C：变参函数
来源：http://xse.xylfe.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xmd.jiagoushi.top

[S30] C：头文件保护
来源：http://bqt.nanxinkj.top

#ifndef X_H
来源：http://ghx.9152youxi.cn

#define X_H
来源：http://ahb.tian-w.cn

#endif
来源：http://sgk.yuxming.cn

[S31] C++：Hello World
来源：http://vcw.yvedp.cn

#include <iostream>
来源：http://mpo.gotoacloud.top

int main() { std::cout << "Hello\n"; }
来源：http://okk.zhiwuduotai.top

[S32] C++：字符串
来源：http://ykq.snrcjt.cn

std::string s = "hi";  s += "!";
来源：http://gcr.wangshuangyany.cn

[S33] C++：vector 增删
来源：http://zlf.yfazqb.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://efs.hesvh.cn

[S34] C++：遍历 vector
来源：http://zgx.xylfe.cn

for (auto &x : v) { std::cout << x; }
来源：http://tdk.yj20258.top

[S35] C++：map
来源：http://tlh.zhijiandao.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mss.jinqigufen.top

[S36] C++：unordered_map
来源：http://lma.fehbvm.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bqd.daxiang520.top

[S37] C++：set
来源：http://mws.ppjwa.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://amu.hysaishi.cn

[S38] C++：排序
来源：http://zfi.cqqwz.cn

std::sort(v.begin(), v.end());
来源：http://rqq.gogol.net.cn


<!-- 参考信息 -->