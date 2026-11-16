代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nae.chenlongwang.top

[Q58] 累计求和
来源：http://jbs.yonumen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tba.yangfankeji.com

[Q59] 分组内累计
来源：http://wou.yuanzhike.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jmb.ctjpmb.com

[Q60] 取上一行 / 下一行
来源：http://voy.daxiang520.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jcl.shzxlz.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://omb.bbcook.cn

[Q61] 移动平均
来源：http://tbj.kuanghao11.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fcy.jqgufenzy.top

[Q62] 分组占比
来源：http://thk.tian-w.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://flv.fehbvm.com

[Q63] 开启事务
来源：http://plb.dianchejie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fvw.yj20258888.top

[Q64] 提交事务
来源：http://jcp.havefunace.top

COMMIT;
来源：http://uor.hcnkem.com

[Q65] 回滚事务
来源：http://bfq.chenzaomai.com

ROLLBACK;
来源：http://ekh.zhiwuduotai.top

[Q66] 行锁查询
来源：http://nvw.yvedp.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qvq.nwbrower.top

[Q67] 设置隔离级别
来源：http://swn.bjfxy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ybq.sjlbkw.cn

[Q68] 保存点
来源：http://gxx.kuanghao11.cn

SAVEPOINT sp1;
来源：http://kjd.sufxvd.cn

ROLLBACK TO sp1;
来源：http://hpu.redwolf501.top

[Q69] 查看执行计划
来源：http://iwz.cashguo.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lru.ehwqpu.com

[Q70] 更新统计信息
来源：http://xto.shanyushiyangtech.top

ANALYZE TABLE users;
来源：http://kft.zhiwuduotai.top

[Q71] 查看建表语句
来源：http://kck.sjlbkw.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://txe.hfpthk.cn

[Q72] 查看索引
来源：http://jvu.zdbjq.cn

SHOW INDEX FROM users;
来源：http://teo.nwbrower.top

[Q73] 查看表状态
来源：http://vpr.fktsv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gmv.pengpengdd.cyou

[Q74] 强制使用索引
来源：http://wtu.xuanzx.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qkl.yuxming.cn

[Q75] 日期格式化
来源：http://ads.chenzaomai.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://oys.yj20258888.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ncp.gotoacloud.top

[Q76] 按天统计
来源：http://pfo.shangyingyoupin.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rub.iojbl.cn

[Q77] 时间加减
来源：http://ywy.nanxinkj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vdx.yueranfly.top

[Q78] 当前时间
来源：http://kqm.yonumen.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://axb.ivvv.top

[Q79] 字符串拼接
来源：http://hlc.hywenlv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://itw.redwolf501.top

[Q80] 字符串截取
来源：http://dgx.xylfe.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mgv.zhixingplan.top

[Q81] 字符串替换
来源：http://osb.shanyushiyangtech.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qqg.zhoulong.xyz

[Q82] 字符长度与字节长度
来源：http://gux.sweek.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vtg.zhaomingkeji.xyz

[Q83] 大小写转换
来源：http://uyi.yonumen.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hbr.yj20258888.top

[Q84] 去除首尾空格
来源：http://qop.smart0.xyz

SELECT TRIM(name) FROM users;
来源：http://lke.ivvv.top

[Q85] 数值取整
来源：http://exh.xinyue.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mfr.xuanzx.com

[Q86] 读取 JSON 字段
来源：http://sge.hnqzz.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jys.tanke756.top

[Q87] JSON 字段做条件
来源：http://unz.cdnleiting.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://udi.daria6918.cn

[Q88] 行转列（条件聚合）
来源：http://uzx.ivvv.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ger.snrcjt.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qgr.pycfn.com

[Q89] 判断表是否存在
来源：http://atm.kuanghao11.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://urz.cdnleiting.top

[Q90] 生成序号列
来源：http://ycp.ydjk.org.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jan.zhaomingkeji.xyz

================================================================================
来源：http://qye.tian-w.cn

R. Bash 专题
来源：http://ngg.jqgfzy.top

================================================================================
来源：http://uvo.cqqwz.cn

[R01] shebang 与严格模式
来源：http://wtp.yanxiufei.cn

#!/usr/bin/env bash
来源：http://cgy.shanyushiyangtech.top

set -euo pipefail
来源：http://ubf.xuetiantiany.cn

[R02] 变量赋值与使用
来源：http://glm.52xcode.cn

name="Tom"; echo "$name"
来源：http://wva.feifeiyinyue.top

[R03] 只读变量
来源：http://uvm.dashuyun.cn

readonly PI=3.14
来源：http://skd.hysaishi.cn

[R04] 位置参数
来源：http://nya.cucudq.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dom.9152youxi.cn

[R05] 参数默认值
来源：http://ten.sxryk.cn

name="${1:-default}"
来源：http://vhx.yongpay.top

[R06] 判断命令是否存在
来源：http://psk.hnxiangtu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rqb.fengsongda.top

[R07] if 判断文件
来源：http://wht.xylfe.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vxc.cashguo.top

[R08] 数值比较
来源：http://hpj.zhoulong.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://vmd.fengsongda.top

[R09] 字符串比较
来源：http://lni.nwbrower.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://drb.zhixingplan.top

[R10] 正则匹配
来源：http://onf.shanyushiyangtech.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ybp.ybcxt.top

[R11] case 多分支
来源：http://hsy.gzhubu.top

case "$1" in
来源：http://vtd.cheryme.top

start) echo "启动" ;;
来源：http://bmw.andypj.xyz

stop)  echo "停止" ;;
来源：http://xhr.bbcook.cn

*)     echo "未知命令" ;;
来源：http://kpg.guowangkeji.top

esac
来源：http://yqb.tarul.cn

[R12] for 遍历文件
来源：http://gwy.hysaishi.cn

for f in *.txt; do echo "$f"; done
来源：http://qfa.jinqigfzy.top

[R13] for 计数循环
来源：http://dnc.zhoulong.xyz

for i in {1..10}; do echo "$i"; done
来源：http://erk.shzxlz.cn

[R14] C 风格 for
来源：http://aeg.gogol.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vln.jyoumei.cn

[R15] while 逐行读文件
来源：http://mzo.vqdsnc.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jrs.ydjk.org.cn

[R16] until 等待条件
来源：http://hjt.jqgfzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hoa.snrcjt.cn

[R17] 数组定义与取值
来源：http://gyn.yfazqb.com

arr=(a b c); echo "${arr[0]}"
来源：http://dyc.shanyushiyangtech.top

[R18] 遍历数组
来源：http://dzy.meibo888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pea.xingfuxueyuan.xyz

[R19] 数组长度
来源：http://ibp.xinyue.icu

echo "${#arr[@]}"
来源：http://dpi.guannengcc.top

[R20] 关联数组（字典）
来源：http://rbc.yangfankeji.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rxl.316326.xyz

[R21] 字符串长度
来源：http://wcu.yongpay.top

echo "${#s}"
来源：http://cmv.tian-w.cn

[R22] 截取子串
来源：http://jra.sysykeji.top

echo "${s:0:5}"
来源：http://rvj.feifeiyinyue.top

[R23] 字符串替换
来源：http://spz.epnwcf.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://oul.316326.xyz

[R24] 大小写转换
来源：http://urb.c1oappe.top

echo "${s^^}"; echo "${s,,}"
来源：http://vug.jianghu66.top

[R25] 去后缀 / 去前缀
来源：http://rxi.aizwys.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yay.ydjk.org.cn

[R26] 命令替换
来源：http://nyr.birdmap.top

now=$(date +%F); echo "$now"
来源：http://qqe.jinghuilouyu.cn

[R27] 算术展开
来源：http://akm.yongpay.top

echo $((1 + 2 * 3))
来源：http://qta.snrcjt.cn

[R28] 浮点运算
来源：http://aij.havefunace.top

echo "scale=2; 10/3" | bc
来源：http://xqi.andypj.xyz

[R29] 定义函数
来源：http://jke.meibo888.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ezs.guowangkeji.top

[R30] 函数返回状态码
来源：http://fsm.sweek.top

f() { return 0; }; f || echo "失败了"
来源：http://tqw.fehbvm.com

[R31] 局部变量
来源：http://oks.cdnleiting.top

f() { local x=1; echo "$x"; }
来源：http://qlb.dashuyun.cn

[R32] 参数个数校验
来源：http://rrc.yueranfly.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mlf.9152youxi.cn

[R33] 捕获错误并提示行号
来源：http://oae.zhijiandao.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wpa.pycfn.com

[R34] 退出时清理
来源：http://jjh.ehwqpu.com

trap 'rm -f "$tmp"' EXIT
来源：http://hav.vehdjk.com

[R35] 后台执行并等待
来源：http://dyd.c1oappe.top

sleep 5 & pid=$!; wait "$pid"
来源：http://bwx.dianchejie.cn

[R36] 并发执行多个任务
来源：http://asu.nwbrower.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kms.shzxlz.cn

[R37] 把输出赋给变量
来源：http://lah.xziqi.cn

files=$(ls -1)
来源：http://moh.zhongyouzk.top

[R38] 管道串联
来源：http://nzc.52xcode.cn

cat a.txt | grep -i error | wc -l
来源：http://und.hnxiangtu.top

[R39] 重定向标准输出与错误
来源：http://ypw.yj20258.top

cmd > out.log 2>&1
来源：http://noy.hcnkem.com

[R40] 追加写日志
来源：http://tsi.sweek.top

echo "log" >> out.log
来源：http://zqw.c1oappe.top

[R41] 丢弃输出
来源：http://duj.jqgufenzy.top

cmd >/dev/null 2>&1
来源：http://pfo.ppjwa.cn

[R42] 输入重定向
来源：http://ulv.yueranfly.top

wc -l < a.txt
来源：http://jve.fengsongda.top

[R43] 按名字查找文件
来源：http://dwm.haohaochexian.top

find . -name "*.log" -type f
来源：http://svi.chenzaomai.com

[R44] 按修改时间查找
来源：http://xvj.316326.xyz

find . -mtime -7 -type f
来源：http://rbv.xuetiantiany.cn

[R45] 批量删除
来源：http://ids.cheryme.top

find . -name "*.tmp" -delete
来源：http://mor.hnxiangtu.top

[R46] 递归替换文件内容
来源：http://jgn.hammf.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ydx.yuxming.cn

[R47] sed 单行替换
来源：http://rqb.quarkkingdee.top

sed -i 's/foo/bar/g' a.txt
来源：http://dei.haohaochexian.top

[R48] awk 取指定列
来源：http://jql.xinyue.icu

awk '{print $1, $3}' a.txt
来源：http://fbh.hcnkem.com

[R49] awk 带条件
来源：http://gfg.shanyushiyangkeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xte.fktsv.cn

[R50] awk 求和
来源：http://ycs.jianghu66.top

awk '{s += $2} END {print s}' a.txt
来源：http://rmc.mhx1999.top

[R51] 排序去重取前几
来源：http://yoh.0kj1m.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://eik.zycfv.cn

[R52] 统计行数
来源：http://waq.jinyuanbaomall.cn

wc -l a.txt
来源：http://vem.cheryme.top

[R53] 查看文件头与实时尾
来源：http://pjg.cheryme.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nmd.jyoumei.cn

[R54] 比较两个文件
来源：http://fqp.zdbjq.cn

diff a.txt b.txt
来源：http://wpm.quarkkingdee.top

[R55] 压缩与解压
来源：http://lpd.wangdashe.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wdu.hongshengwenyu.top

[R56] 远程拷贝
来源：http://yrn.tian-w.cn

scp file user@host:/path/
来源：http://lbq.hywenlv.cn

[R57] 远程执行命令
来源：http://ymk.sufxvd.cn

ssh user@host 'uptime'
来源：http://dwk.daxiang520.top

[R58] 下载文件
来源：http://lty.guowangkeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nfj.ctjpmb.com

[R59] 发 POST JSON
来源：http://xhb.zhixingplan.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hnx.chenjidiqi.icu

[R60] 只看 HTTP 状态码
来源：http://umk.fzhhl.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yfi.bjfxy.top

[R61] 磁盘占用
来源：http://kll.jqgfzy.top

df -h;  du -sh *
来源：http://cib.nanxinkj.top

[R62] 找最占空间的文件
来源：http://guj.feifeiyinyue.top

du -ah . | sort -rh | head -10
来源：http://bgo.sxryk.cn

[R63] 内存与进程
来源：http://qlw.bjfxy.top

free -h;  ps aux | grep nginx
来源：http://jsj.yonumen.top

[R64] 结束进程
来源：http://zkp.jinyuanbaomall.cn

kill -9 $(pgrep -f app.py)
来源：http://jep.tian-w.cn

[R65] 查看端口占用
来源：http://mbe.jinyuanbaomall.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hrz.316326.xyz

[R66] 定时任务
来源：http://ytr.chenjidiqi.icu

crontab -e;  crontab -l
来源：http://cij.bjfxy.top

[R67] 生成随机十六进制串
来源：http://euk.jianghu66.top

openssl rand -hex 16
来源：http://tcn.aibaodan.cn

[R68] 计算文件校验值
来源：http://bxx.cucudq.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tqo.xuetiantiany.cn

[R69] 生成随机密码
来源：http://egd.zhoulong.xyz

head -c 16 /dev/urandom | base64
来源：http://jyr.uphjek.com

[R70] 时间戳与互转
来源：http://smb.yj202588.top

date +%s;  date -d @1700000000
来源：http://yxs.shanyushiyangkeji.top

[R71] 日期格式化
来源：http://nlr.ybcxt.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://cig.yangfankeji.com

[R72] 等待端口就绪
来源：http://uml.jinghuilouyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dkw.svipenyu.cn

[R73] 分割大日志
来源：http://gcr.sweek.top

split -l 1000 big.log part_
来源：http://xho.yfazqb.com

[R74] 批量重命名
来源：http://qrg.snrcjt.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://umh.zhoulong.xyz

[R75] 导出环境变量
来源：http://kxw.xuetiantiany.cn

export PATH="$HOME/bin:$PATH"
来源：http://njq.yongpay.top

[R76] 使用临时文件
来源：http://djt.jinghuilouyu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://isx.shangyingyoupin.top

[R77] 读取用户输入
来源：http://hdb.chenlongwang.top

read -rp "请输入: " ans
来源：http://mde.yj202588.top

[R78] 交互式菜单
来源：http://hbw.ctjpmb.com

select opt in a b c; do echo "$opt"; break; done
来源：http://kiw.nanxinkj.top

[R79] 解析命令行选项
来源：http://tpw.wangshuangyany.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://coz.epnwcf.com

[R80] 查看脚本执行耗时
来源：http://trl.yj20258888.top

time ./run.sh
来源：http://fei.cashguo.top

================================================================================
来源：http://jsn.52xcode.cn

S. C / C++ 专题
来源：http://uor.hnxiangtu.top

================================================================================
来源：http://ria.dianchejie.cn

[S01] C：Hello World
来源：http://qgi.ppjwa.cn

#include <stdio.h>
来源：http://lbm.quarkkingdee.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://dtp.zhijiandao.cn

[S02] C：变量与格式化输出
来源：http://kmn.daria6918.cn

int a = 10; printf("%d\n", a);
来源：http://qpn.hcnkem.com

[S03] C：读入整数
来源：http://jyj.jyoumei.cn

int x; scanf("%d", &x);
来源：http://deu.0kj1m.cn

[S04] C：字符串复制
来源：http://dtc.fanxiaobao.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://cpi.xuetiantiany.cn

[S05] C：字符串长度
来源：http://egc.zdbjq.cn

strlen(s)
来源：http://cap.chenlongwang.top

[S06] C：字符串比较
来源：http://agl.zycfv.cn

strcmp(a, b) == 0
来源：http://leh.chenlongwang.top

[S07] C：数组遍历求和
来源：http://kld.yanxiufei.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zal.fktsv.cn

[S08] C：动态内存分配与释放
来源：http://zix.zdbjq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blc.ivvv.top

[S09] C：结构体定义与初始化
来源：http://gzj.xuetiantiany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pso.tanke756.top

[S10] C：指针与解引用
来源：http://ekc.zhoulong.xyz

int *p = &a;  *p = 5;
来源：http://mbo.zhoulong.xyz

[S11] C：逐行读文件
来源：http://btv.jlsjyb.cn

FILE *f = fopen("a.txt", "r");
来源：http://ugq.sysykeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://gll.yangfankeji.com

fclose(f);
来源：http://oet.jinqigfzy.top

[S12] C：写文件
来源：http://tdg.hcnkem.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vwq.shuidangran.top

[S13] C：宏定义
来源：http://nuq.sjlbkw.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jhi.ydzc1.top

[S14] C：枚举
来源：http://hue.zdbjq.cn

enum Color { RED, GREEN, BLUE };
来源：http://fjg.yuxming.cn

[S15] C：类型转换
来源：http://vdn.zycfv.cn

(double) a / b
来源：http://oca.dashuyun.cn

[S16] C：位操作置位
来源：http://yfu.aibaodan.cn

x |= (1 << 3);
来源：http://pke.fzhhl.top

[S17] C：安全拼接字符串
来源：http://rkp.vqdsnc.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://boy.c1oappe.top

[S18] C：命令行参数
来源：http://kpl.haohaochexian.top

int main(int argc, char **argv)
来源：http://ykt.cdnleiting.top

[S19] C：快速排序
来源：http://ocb.ybcxt.top

qsort(a, n, sizeof(int), cmp);
来源：http://lhi.hnqzz.top

[S20] C：二分查找
来源：http://dvi.wangshuangyany.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pkr.hnxiangtu.top

[S21] C：字符类别判断
来源：http://kbt.xingfuxueyuan.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yvf.yfazqb.com

[S22] C：字符串转数字
来源：http://kcq.sxryk.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lgl.yuxming.cn

[S23] C：随机数
来源：http://wiw.jinyuanbaomall.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://les.yj20258.top

[S24] C：获取本地时间
来源：http://mtn.shuidangran.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rwf.havefunace.top

[S25] C：内存拷贝
来源：http://tbv.fktsv.cn

memcpy(dst, src, n);
来源：http://yfc.jyoumei.cn

[S26] C：内存清零
来源：http://zea.gaohongyu789.top

memset(a, 0, sizeof a);
来源：http://ssk.jlsjyb.cn

[S27] C：定义常量
来源：http://nnx.guowangkeji.top

const double PI = 3.14159;
来源：http://pyk.tian-w.cn

[S28] C：静态变量
来源：http://mdk.uphjek.com


<!-- 参考信息 -->