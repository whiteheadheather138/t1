代发 wailian999

[Q63] 开启事务
来源：http://qmq.sweek.top

START TRANSACTION;                -- 或 BEGIN
来源：http://rpd.wangdashe.top

[Q64] 提交事务
来源：http://pvr.yj20258.top

COMMIT;
来源：http://bsf.tanke756.top

[Q65] 回滚事务
来源：http://qif.zdbjq.cn

ROLLBACK;
来源：http://afg.ctjpmb.com

[Q66] 行锁查询
来源：http://siv.jinghuilouyu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wkq.zdbjq.cn

[Q67] 设置隔离级别
来源：http://wtb.guowangkeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dwd.sufxvd.cn

[Q68] 保存点
来源：http://pcb.jyoumei.cn

SAVEPOINT sp1;
来源：http://zja.vqdsnc.cn

ROLLBACK TO sp1;
来源：http://rsg.ybcxt.top

[Q69] 查看执行计划
来源：http://rzp.xuanzx.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mbu.zhengqikj.top

[Q70] 更新统计信息
来源：http://tej.meibo888.top

ANALYZE TABLE users;
来源：http://lxp.pengpengdd.cyou

[Q71] 查看建表语句
来源：http://its.mhx1999.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xaa.yonumen.top

[Q72] 查看索引
来源：http://pzj.hammf.cn

SHOW INDEX FROM users;
来源：http://ggw.meibo888.top

[Q73] 查看表状态
来源：http://ugc.gzhubu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://poh.zhaomingkeji.xyz

[Q74] 强制使用索引
来源：http://wpk.zhoulong.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bye.shanyushiyangtech.top

[Q75] 日期格式化
来源：http://icy.zhijiandao.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tnt.wangdashe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ofy.fehbvm.com

[Q76] 按天统计
来源：http://nct.9152youxi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wlq.yanxiufei.cn

[Q77] 时间加减
来源：http://wps.svipenyu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zoi.tian-w.cn

[Q78] 当前时间
来源：http://eqk.chenjidiqi.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gyt.nanxuanxn.top

[Q79] 字符串拼接
来源：http://uqw.andypj.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bkp.jinyuanbaomall.cn

[Q80] 字符串截取
来源：http://fjr.yuanzhike.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bnb.dianchejie.cn

[Q81] 字符串替换
来源：http://vxd.smart0.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wgf.haohaochexian.top

[Q82] 字符长度与字节长度
来源：http://iyh.yongpay.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ywk.jinghuilouyu.cn

[Q83] 大小写转换
来源：http://pwn.dashuyun.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mvt.zhongyouzk.top

[Q84] 去除首尾空格
来源：http://fxr.tian-w.cn

SELECT TRIM(name) FROM users;
来源：http://has.pycfn.com

[Q85] 数值取整
来源：http://tjh.jqgufenzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hqh.jinyuanbaomall.cn

[Q86] 读取 JSON 字段
来源：http://rbe.hcnkem.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jxv.chenzaomai.com

[Q87] JSON 字段做条件
来源：http://wpn.sxryk.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ipq.nanxuanxn.top

[Q88] 行转列（条件聚合）
来源：http://xom.jyoumei.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bkb.chenjidiqi.icu

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ljw.bbcook.cn

[Q89] 判断表是否存在
来源：http://ojd.haohaochexian.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dtm.aibaodan.cn

[Q90] 生成序号列
来源：http://jbu.tianlin.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jwh.316326.xyz

================================================================================
来源：http://hcz.shangyingyoupin.top

R. Bash 专题
来源：http://xlj.nanxinkj.top

================================================================================
来源：http://kwf.hcnkem.com

[R01] shebang 与严格模式
来源：http://pkp.zhijiandao.cn

#!/usr/bin/env bash
来源：http://wau.yvedp.cn

set -euo pipefail
来源：http://nwx.jianghu66.top

[R02] 变量赋值与使用
来源：http://ewp.fengsongda.top

name="Tom"; echo "$name"
来源：http://svx.316326.xyz

[R03] 只读变量
来源：http://zqz.sweek.top

readonly PI=3.14
来源：http://ekn.cdnleiting.top

[R04] 位置参数
来源：http://zmc.sufxvd.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lri.316326.xyz

[R05] 参数默认值
来源：http://fij.shangyingyoupin.top

name="${1:-default}"
来源：http://eyp.tian-w.cn

[R06] 判断命令是否存在
来源：http://djy.yvedp.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vzm.sufxvd.cn

[R07] if 判断文件
来源：http://xkx.ydzc1.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rsq.zhongyouzk.top

[R08] 数值比较
来源：http://olz.ehwqpu.com

if (( a > b )); then echo "a 更大"; fi
来源：http://jyh.wangdashe.top

[R09] 字符串比较
来源：http://zcl.chenlongwang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bxn.ivvv.top

[R10] 正则匹配
来源：http://bhv.wangshuangyany.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hou.xziqi.cn

[R11] case 多分支
来源：http://yus.hfpthk.cn

case "$1" in
来源：http://dmm.jinqigufen.top

start) echo "启动" ;;
来源：http://fnv.sweek.top

stop)  echo "停止" ;;
来源：http://hkq.sjlbkw.cn

*)     echo "未知命令" ;;
来源：http://shm.yfazqb.com

esac
来源：http://bda.hesvh.cn

[R12] for 遍历文件
来源：http://tug.hywenlv.cn

for f in *.txt; do echo "$f"; done
来源：http://zpy.dashuyun.cn

[R13] for 计数循环
来源：http://kjw.pycfn.com

for i in {1..10}; do echo "$i"; done
来源：http://udn.birdmap.top

[R14] C 风格 for
来源：http://amp.ppjwa.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dpv.shanyushiyangtech.top

[R15] while 逐行读文件
来源：http://qcu.jyoumei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fag.xuetiantiany.cn

[R16] until 等待条件
来源：http://jpu.zhixingplan.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ocg.nanxuanxn.top

[R17] 数组定义与取值
来源：http://cpx.ivvv.top

arr=(a b c); echo "${arr[0]}"
来源：http://muc.jinghuilouyu.cn

[R18] 遍历数组
来源：http://rdl.yanxiufei.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ygd.uphjek.com

[R19] 数组长度
来源：http://slc.zhiwuduotai.top

echo "${#arr[@]}"
来源：http://ztb.daxiang520.top

[R20] 关联数组（字典）
来源：http://uis.guannengcc.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oso.zhijiandao.cn

[R21] 字符串长度
来源：http://cdw.sufxvd.cn

echo "${#s}"
来源：http://ovm.hammf.cn

[R22] 截取子串
来源：http://fyi.yj202588.top

echo "${s:0:5}"
来源：http://kyb.havefunace.top

[R23] 字符串替换
来源：http://rxw.nanxinkj.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cao.guannengcc.top

[R24] 大小写转换
来源：http://pgx.birdmap.top

echo "${s^^}"; echo "${s,,}"
来源：http://fab.zdqjudy.top

[R25] 去后缀 / 去前缀
来源：http://woo.c1oappe.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://psk.cheryme.top

[R26] 命令替换
来源：http://yob.nanxinkj.top

now=$(date +%F); echo "$now"
来源：http://zlw.zdbjq.cn

[R27] 算术展开
来源：http://kra.ybcxt.top

echo $((1 + 2 * 3))
来源：http://bkg.yongpay.top

[R28] 浮点运算
来源：http://kiw.xziqi.cn

echo "scale=2; 10/3" | bc
来源：http://ytl.fzhhl.top

[R29] 定义函数
来源：http://lzc.jinqigufen.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://juf.sxryk.cn

[R30] 函数返回状态码
来源：http://jjx.yuanzhike.top

f() { return 0; }; f || echo "失败了"
来源：http://yat.jinyuanbaomall.cn

[R31] 局部变量
来源：http://yev.zdqjudy.top

f() { local x=1; echo "$x"; }
来源：http://kxx.birdmap.top

[R32] 参数个数校验
来源：http://ypu.daria6918.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://adv.shuidangran.top

[R33] 捕获错误并提示行号
来源：http://vqq.tanke756.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dml.nanxinkj.top

[R34] 退出时清理
来源：http://zhs.zhiwuduotai.top

trap 'rm -f "$tmp"' EXIT
来源：http://qjm.feifeiyinyue.top

[R35] 后台执行并等待
来源：http://hlx.cucudq.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zqe.xylfe.cn

[R36] 并发执行多个任务
来源：http://jxi.guowangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gtt.yuxming.cn

[R37] 把输出赋给变量
来源：http://lvi.uphjek.com

files=$(ls -1)
来源：http://xqr.chenzaomai.com

[R38] 管道串联
来源：http://phj.bjfxy.top

cat a.txt | grep -i error | wc -l
来源：http://flz.feifeiyinyue.top

[R39] 重定向标准输出与错误
来源：http://drh.cdnleiting.top

cmd > out.log 2>&1
来源：http://zoz.jinyuanbaomall.cn

[R40] 追加写日志
来源：http://ntu.ydjk.org.cn

echo "log" >> out.log
来源：http://fop.cashguo.top

[R41] 丢弃输出
来源：http://uys.uphjek.com

cmd >/dev/null 2>&1
来源：http://sik.jlsjyb.cn

[R42] 输入重定向
来源：http://bew.0kj1m.cn

wc -l < a.txt
来源：http://dlx.shanyushiyangkeji.top

[R43] 按名字查找文件
来源：http://ecb.dianchejie.cn

find . -name "*.log" -type f
来源：http://bvp.dianchejie.cn

[R44] 按修改时间查找
来源：http://lve.sweek.top

find . -mtime -7 -type f
来源：http://woz.yvedp.cn

[R45] 批量删除
来源：http://jxw.yj20258888.top

find . -name "*.tmp" -delete
来源：http://hxh.epnwcf.com

[R46] 递归替换文件内容
来源：http://qhj.hammf.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rzc.gzhubu.top

[R47] sed 单行替换
来源：http://oby.shuidangran.top

sed -i 's/foo/bar/g' a.txt
来源：http://sxh.vehdjk.com

[R48] awk 取指定列
来源：http://gmk.daria6918.cn

awk '{print $1, $3}' a.txt
来源：http://bxw.zhiwuduotai.top

[R49] awk 带条件
来源：http://wxm.jiagoushi.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vcg.snrcjt.cn

[R50] awk 求和
来源：http://eql.xinyue.icu

awk '{s += $2} END {print s}' a.txt
来源：http://ujp.havefunace.top

[R51] 排序去重取前几
来源：http://hit.chenzaomai.com

sort a.txt | uniq -c | sort -rn | head
来源：http://gny.zycfv.cn

[R52] 统计行数
来源：http://pdd.svipenyu.cn

wc -l a.txt
来源：http://vgz.ivvv.top

[R53] 查看文件头与实时尾
来源：http://wms.zycfv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://klq.nwbrower.top

[R54] 比较两个文件
来源：http://ymy.smart0.xyz

diff a.txt b.txt
来源：http://nbq.ydjk.org.cn

[R55] 压缩与解压
来源：http://uon.zdqjudy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://amb.9152youxi.cn

[R56] 远程拷贝
来源：http://izf.yj202588.top

scp file user@host:/path/
来源：http://pon.shuidangran.top

[R57] 远程执行命令
来源：http://eoy.aizwys.cn

ssh user@host 'uptime'
来源：http://luk.vehdjk.com

[R58] 下载文件
来源：http://rlf.ywan-chungtsiang.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mxx.cucudq.cn

[R59] 发 POST JSON
来源：http://pel.wangdashe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bho.zhiwuduotai.top

[R60] 只看 HTTP 状态码
来源：http://lbw.gzhubu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dnp.hesvh.cn

[R61] 磁盘占用
来源：http://jhd.9152youxi.cn

df -h;  du -sh *
来源：http://cwo.nanxinkj.top

[R62] 找最占空间的文件
来源：http://xli.cucudq.cn

du -ah . | sort -rh | head -10
来源：http://fel.guannengcc.top

[R63] 内存与进程
来源：http://vxq.52xcode.cn

free -h;  ps aux | grep nginx
来源：http://gxb.jqgufenzy.top

[R64] 结束进程
来源：http://inz.snrcjt.cn

kill -9 $(pgrep -f app.py)
来源：http://nhx.xuanzx.com

[R65] 查看端口占用
来源：http://iia.uphjek.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uqn.fzhhl.top

[R66] 定时任务
来源：http://rmh.hfpthk.cn

crontab -e;  crontab -l
来源：http://ecl.sweek.top

[R67] 生成随机十六进制串
来源：http://zvg.cqqwz.cn

openssl rand -hex 16
来源：http://bzq.nanxuanxn.top

[R68] 计算文件校验值
来源：http://cdz.haohaochexian.top

sha256sum a.txt;  md5sum a.txt
来源：http://gdy.xziqi.cn

[R69] 生成随机密码
来源：http://rqm.yonumen.top

head -c 16 /dev/urandom | base64
来源：http://nev.hesvh.cn

[R70] 时间戳与互转
来源：http://szo.jinqigufen.top

date +%s;  date -d @1700000000
来源：http://fyd.cheryme.top

[R71] 日期格式化
来源：http://qqn.shuidangran.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://tam.zhoulong.xyz

[R72] 等待端口就绪
来源：http://ogl.gotoacloud.top

until nc -z localhost 3306; do sleep 1; done
来源：http://lge.shzxlz.cn

[R73] 分割大日志
来源：http://ftb.nanxinkj.top

split -l 1000 big.log part_
来源：http://cnk.dashuyun.cn

[R74] 批量重命名
来源：http://xow.nanxinkj.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mki.cqqwz.cn

[R75] 导出环境变量
来源：http://ttt.jianghu66.top

export PATH="$HOME/bin:$PATH"
来源：http://aaj.xuanzx.com

[R76] 使用临时文件
来源：http://cnm.ctjpmb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dzp.ywan-chungtsiang.top

[R77] 读取用户输入
来源：http://qoe.feifeiyinyue.top

read -rp "请输入: " ans
来源：http://kfo.zhaomingkeji.xyz

[R78] 交互式菜单
来源：http://vvx.daxiang520.top

select opt in a b c; do echo "$opt"; break; done
来源：http://oiv.zhixingplan.top

[R79] 解析命令行选项
来源：http://iez.yvedp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rol.yueranfly.top

[R80] 查看脚本执行耗时
来源：http://kjx.zycfv.cn

time ./run.sh
来源：http://ceh.tianlin.xyz

================================================================================
来源：http://hcv.mhx1999.top

S. C / C++ 专题
来源：http://qui.0kj1m.cn

================================================================================
来源：http://cwf.yuxming.cn

[S01] C：Hello World
来源：http://wdn.xingfuxueyuan.xyz

#include <stdio.h>
来源：http://qui.kuanghao11.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://iki.sjlbkw.cn

[S02] C：变量与格式化输出
来源：http://hdr.zhaomingkeji.xyz

int a = 10; printf("%d\n", a);
来源：http://cwh.hongshengwenyu.top

[S03] C：读入整数
来源：http://kjf.sysykeji.top

int x; scanf("%d", &x);
来源：http://mjc.xuetiantiany.cn

[S04] C：字符串复制
来源：http://lvp.gotoacloud.top

char dst[32]; strcpy(dst, "hi");
来源：http://npl.hammf.cn

[S05] C：字符串长度
来源：http://etc.chenlongwang.top

strlen(s)
来源：http://akz.vqdsnc.cn

[S06] C：字符串比较
来源：http://rlu.gogol.net.cn

strcmp(a, b) == 0
来源：http://rss.yanxiufei.cn

[S07] C：数组遍历求和
来源：http://gjj.xingfuxueyuan.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zbt.xuetiantiany.cn

[S08] C：动态内存分配与释放
来源：http://ewp.yanxiufei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ohi.hysaishi.cn

[S09] C：结构体定义与初始化
来源：http://pfs.bbcook.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://aid.hongshengwenyu.top

[S10] C：指针与解引用
来源：http://pvo.epnwcf.com

int *p = &a;  *p = 5;
来源：http://lev.quarkkingdee.top

[S11] C：逐行读文件
来源：http://lah.hywenlv.cn

FILE *f = fopen("a.txt", "r");
来源：http://ynj.tianlin.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://rtm.iojbl.cn

fclose(f);
来源：http://uac.svipenyu.cn

[S12] C：写文件
来源：http://qfz.redwolf501.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fgk.xylfe.cn

[S13] C：宏定义
来源：http://tzy.yangfankeji.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cpc.9152youxi.cn

[S14] C：枚举
来源：http://kml.yvedp.cn

enum Color { RED, GREEN, BLUE };
来源：http://wva.wangshuangyany.cn

[S15] C：类型转换
来源：http://xva.snrcjt.cn

(double) a / b
来源：http://yes.zhijiandao.cn

[S16] C：位操作置位
来源：http://mle.jianghu66.top

x |= (1 << 3);
来源：http://yak.vqdsnc.cn

[S17] C：安全拼接字符串
来源：http://kpp.yangfankeji.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lzh.52xcode.cn

[S18] C：命令行参数
来源：http://lwy.meibo888.top

int main(int argc, char **argv)
来源：http://sjs.hammf.cn

[S19] C：快速排序
来源：http://xsi.jqgufenzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://sbk.hesvh.cn

[S20] C：二分查找
来源：http://bex.zycfv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pkk.jiagoushi.top

[S21] C：字符类别判断
来源：http://lxp.wangdashe.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ovr.yanxiufei.cn

[S22] C：字符串转数字
来源：http://rzl.jyoumei.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wdp.birdmap.top

[S23] C：随机数
来源：http://tvz.xuanzx.com

srand(time(NULL));  int r = rand() % 100;
来源：http://kss.zdqjudy.top

[S24] C：获取本地时间
来源：http://wvy.ywan-chungtsiang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://txr.pycfn.com

[S25] C：内存拷贝
来源：http://hnc.dianchejie.cn

memcpy(dst, src, n);
来源：http://lmh.yonumen.top

[S26] C：内存清零
来源：http://lpx.fzhhl.top

memset(a, 0, sizeof a);
来源：http://gwz.fzhhl.top

[S27] C：定义常量
来源：http://ksh.shangyingyoupin.top

const double PI = 3.14159;
来源：http://htd.gogol.net.cn

[S28] C：静态变量
来源：http://xxx.gzhubu.top

static int counter = 0;
来源：http://uix.fengsongda.top

[S29] C：变参函数
来源：http://gfi.fehbvm.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rro.fzhhl.top

[S30] C：头文件保护
来源：http://qkd.xinyue.icu

#ifndef X_H
来源：http://dtn.zhixingplan.top

#define X_H
来源：http://efu.chenjidiqi.icu

#endif
来源：http://ozh.xuanzx.com

[S31] C++：Hello World
来源：http://kjy.quarkkingdee.top

#include <iostream>
来源：http://ntv.gotoacloud.top

int main() { std::cout << "Hello\n"; }
来源：http://tmo.vqdsnc.cn

[S32] C++：字符串
来源：http://wmd.snrcjt.cn

std::string s = "hi";  s += "!";
来源：http://tle.snrcjt.cn


<!-- 参考信息 -->